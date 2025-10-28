# Battery-Alert
Working : Notifies when battery level of windows system reaches more than 98%

Steps to Follow : 
1. download and extract "Batterypercentage" file - it contains Readme file, Battery.rar, 6 images
2. extract "battery.rar" file which is inside "Batterypercentage" folder and copy this to your local drive - it contatins Runsilent.vbs & BatteryAlert.ps1
3. get the path of "BatteryAlert.ps1"
4. edit "Runsilent.vbs" on notepad and change "C:\Battery\BatteryAlert.ps1" with the location of your copied location
5. check wthether the location of "BatteryAlert.ps1" is correctly mentioned in "Runsilent.vbs"
6. open task scheduler using start menu
7. create task and follow settings like the images 0 to 5

   "0.png" - click create task
   
   "1.png" - General tab - give your preferred name
   
   "2.png" - Triggers tab - clcik new - select daily - give any time - recur 1 days - repeat task every 30 mins - if you want you can change time value to 30 mins or 1 hr
   
   "3.png" - Actions tab" - click new - start a program - Enter "wscript.exe" in the box - Add the file location of "Runsilent.vbs" in arguments box
   
   "4.png" & "5.png"- select these settings
   
9. close task scheduler
10. that's all - it will now run during charging and notifies when your charge reached above 98%

Extras :
1. if you want to change battery percentage alert value to any other value other than 98 percentage then change value in the "BatteryAlert.ps1"

   "**98**" is the checking value change this to your preferred value

   "~ge" means "greater than or equal to"

   "~gt" means "greater than"

   "~le" means "less than or equal to"

   "~lt" means "less than"

   "~eq" means "equal to"
