# Budu-Drive-Letter-Utility
<br><br>
##> About Software: ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~
<br><br>
1- AS a utility to help and easy to change the partitions drive letter,
   support 8 partitions at one time<br>
2- Can be used to manage many External USB HDD drive letter<br>
3- Have a function to set partitions data and autofill partitions and letter as in seting<br>
   Every time you conect USB HDD even different computers<br>
4- Suitable for use as portable software which runs from the External HDD or USB Flashdrive<br>
<br><br><br>

##> How BuduDriveLeterUtility Works : ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~
<br><br>
  In the basic, BuduDriveLeterUtility.exe run cmd.exe Diskpart system OS windows to get all the partition drive
  data which is connected to the computer. Data from cmd Diskpart processed and compared with data
  stored in Ini Configurations setting, Then all partitions list which has been processed is filled
  into the combobox for Confirmation, After receiving confirmation (submit), the software will write
  2 file inside System Temp folder, AssignDriveLetter.bat and AssignDriveLetter.txt, Confirmation again
  to run AssignDriveLetter.bat with cmd.exe(Windows OS system)
<br>
  cmd.exe is Default OS Windows Utility to manage partitions and other tasks via command
<br>
  If you only want to see cmd command to be run, press 'Cencel' on the Confirmation Windows,
  And open Temp System folder: C:\Users\User\AppData\Local\Temp\~_BuduDriveLeterUtility\
<br><br><br>

##> How to Use: ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~
<br><br>
For normal use, run the software, select patititions, assign a drive letter, and press submit button and confirmation button to change the drive letter as chosen.<br><br>
For repeated use or has many external (USB) hdd and partition drive to be assigned a drive letter, The save data partitions according to use. Whenever BuduDriveLetterUtility executed when External HDD is connected, the software will autofill combobox as specified in the settings, simply press 'Submit' and confirmation button to change drive letter.
