; --------------------------------------------------
; Name: Budu Drive Letter Utility
; Version: V1.0
; Author: Edy Yussuf
; --------------------------------------------------
 (In the construction and Improvement)

My English not so good to write more

##> About Software: ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~

1- In the foundation as a utility to help and easy to change the partitions drive letter,
   support 8 partitions at one time
2- Can be used to manage many External USB HDD drive letter
3- Have a function to set partitions data and autofill partitions and letter as in seting
   Every time you conect USB HDD even different computers
4- Suitable for use as portable software which runs from the External HDD or USB Flashdrive


##> How BuduDriveLeterUtility Works : ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~

  In the basic, BuduDriveLeterUtility.exe run cmd.exe Diskpart system OS windows to get all the partition drive
  data which is connected to the computer. Data from cmd Diskpart processed and compared with data
  stored in Ini Configurations setting, Then all partitions list which has been processed is filled
  into the combobox for Confirmation, After receiving confirmation (submit), the software will write
  2 file inside System Temp folder, AssignDriveLetter.bat and AssignDriveLetter.txt, Confirmation again
  to run AssignDriveLetter.bat with cmd.exe(Windows OS system)

  cmd.exe is Default OS Windows Utility to manage partitions and other tasks via command

  If you only want to see cmd command to be run, press 'Cencel' on the Confirmation Windows,
  And open Temp System folder: C:\Users\User\AppData\Local\Temp\~_BuduDriveLeterUtility\


##> How to Use: ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~

For normal use, run the software, select patititions, assign a drive letter, and press submit button and confirmation button to change the drive letter as chosen.
For repeated use or has many external (USB) hdd and partition drive to be assigned a drive letter, The save data partitions according to use. Whenever BuduDriveLetterUtility executed when External HDD is connected, the software will autofill combobox as specified in the settings, simply press 'Submit' and confirmation button to change drive letter.


##> Information Configurations And Settings : ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~

checkBox:
1-"Close Windows After Submit"
  Close windows when the BuduDriveLetterUtility.exe process is completed
2-"Skip AutoFill Drive Alredy Assign Letter As In Seting Ini"
  Ignoring such as partitions that are stored in this setting, If you have more
  than 8 partitions want to change it together, this box is checked according to
  gave way to autofill next partitions for a second process
3-"Pause Cmd Window After Finish"
  Close Cmd.exe windows manually
4-"Hide Cmd Windows"
  Run Cmd.exe quietly
5-"Run Program In Text Box After Submit"
  run automatically filled Programs Path in textbox below after completion/finish
6-"Program in same drive ( Using As Portable In USB Drive )"
  The program, which is filled in the textbox below on the same partition
  BuduDriveLetterUtility.exe (partition in the list to change the drive letter(use as Portable)

TextBox:
7-Textbox for the Program Path to executed after completion


##> Info Data Partitions Drive and Example: ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~

 F=0CR708D2-323GB-Document

 F         : Partition Drive Letter
 0CR708D2  : Partition Serial Number
 323GB     : Partition Size
 Document  : Partition Name

 If the data in the 'All Partitions Drive Data',
   F : is the drive letter that is being used by the computer

 If the data in the box 'Ini Seting Partitions Drive Letter' (and 'Drive Data in Settings Ini')
   F : is the drive letter will be changed to F during the process

 Examples of data format that can be used to be stored in Ini setting,
 Example Partitions F above want to Assign Letter to Q

  Q=0CR708D2
  Q=0CR708D2-323
  Q=0CR708D2-323GB
  or data with full name
  Q=0CR708D2-323GB-Document

 Depending on the needs and caving, for example partitions have serial
 and the same size (clone partitions or HDD / duplicate), if necessary change the name
 of the duplicate partitions and use the data in full format : Q=0CR708D2-323GB-New Name


##> How to Save Partitions Drive Data : ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~

For example :
 If you have the 2 USB HDD (or more) that you want to assign a partitions drive
 the same letter even be used on different computers.
  HDD 1 has 4 Partitions, partitions 1 = Q, partitions 2 = U, partitions 3 = R, partitions 2 = S
  HDD 2 has 3 Partitions, partitions 1 = Q, partitions 2 = R, partitions 3 = S

Caution:
 * If the USB HDD is used together at one time, software only autofill partitions
  most of partitions and not in the second set of the same letter. you must
  assign a different drive letter each partitions,
  In this example, two separate USB HDD is used, not used in one time.

 * For safety, Close all folders, files and software from partitions to be
  change drive letter, If the BuduDriveLetterUtility.exe is used as portable in
  external HDD, see guidance at no 1 below

1-Connect the HDD 1 in the computer, wait a few seconds for the computer to detect the USB HDD

 * In this example, the software used as portable and BuduDriveLetterUtility.exe stored in
  Partitions one of the two HDD 1 and HDD 2,
  Open Partition 1 wherein the software stored and run the BuduDriveLetterUtility.exe
  and closing windows explorer.

2-After Run Software, wait a few seconds until the text message 'Wait!' under the lost,
  go to the 'Drive Settings' tab, Press 'All Drive Info' button to open the windows
  information and data on all partitions connected to the computer

3-Box above, the information Windows Diskpart, the 'Drive Data in Settings Ini' to
  displaying data in setting And 'All Partitions Drive Data' displays all partitions data
  which is connected to the computer in BuduDriveLetterUtility.exe setting format

4-Select and copy the 4 partitions data HDD 1 in the box 'All Partitions Drive Data'
  (The most common 4 below) and paste it into the box 'Ini Seting Partitions Drive Letter'
  at the main windows, Change drive letter (the first alphabet of), for example:
  partition 1: E=74ED41E0-106GB-Backup 1, change to Q=74ED41E0-106GB-Backup 1
  partition 2: F=0CR708D2-323GB-Document, change to U=0CR708D2-323GB-Document
  The next variable partition 3 to R and the partition 4 to S
  and Press the 'Save Settings' button.

5-Open Tab 'Drive Manager' and click 'Refresh' button, wait a few seconds for the software
  processing data, and software will autofill combobox with data such as the
  has been set in the above settings. review petitions and letter, make sure it is correct
  Partitions Drive in combobox(Left) and(change to) Letter(Right)

 Finish Set Ini Seting For HDD 1,(for HDD 2 repeat the same process as above)
 below how to change drive letter

6-Press the button 'Submit', Cmd.exe confirmation windows will open and display information
  partitions for confirmation, check again petitions and letter data,
  press 'OK' to continue the process (the 'Cencel' to cancel the process)

7-Window BuduDriveLetterUtility will be closed to make way process and Windows Cmd.exe
  would open the process to change the drive letter partitions, wait for it to finish,
  by default Windows Cmd will be closed when finished, if not closed
  press enter to close it. (maybe pause the box marked in settings,
  Open the tab "Configurations" and uncheck the box "Pause Cmd Window After Finish")

8-Depending on the settings on the tab "Configurations", if the "Close Windows After Submit"
  not marked, Window BuduDriveLetterUtility will open automatically after Windows Cmd.exe closed,
  now All partitions letter HDD 1 change to Q U R S

9-Complete change drive letter partitions HDD 1.


  Now Every time you conect HDD 1 Or HDD 2 even different computers and need change drive letter,
  do step 1, BuduDriveLetterUtility.exe autofilled combobox, make sure it is correct partitions and letter,
  (or chose other letter if you want) and press Submit button like step 6




