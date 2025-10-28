# Battery-Alert
Working : Notifies when battery level of windows system reaches more than 98%

Steps to Follow : 
1. download "Battery.rar" file
2. extract to your local drive
3. Edit "Runsilent.vbs" and change "C:\Battery\BatteryAlert.ps1" with your local copied location
4. open task scheduler using start menu
5. create basic task and give settings like the images 0 to 5
   "0.png" - click create task
   "1.png" - General tab - give your preferred name
   "2.png" - Triggers tab - clcik new - select daily - give any time - recur 1 days - repeak task every 20 mins - if you want you can change this value
   "3.png" - Actions.png" - click new - start a program - Enter "wscript.exe" in the box - Add the file location of "Runsilent.vbs" in arguments box
   "4.png" & "5.png"- select these settings
7. close task scheduler
8. that's all - it will now run during charge and notifies when your charge reached above 98%

Extras :
1. if you want to change battery percentage other than 98 percentage change value in the "BatteryAlert.ps1"
   "**98** to your value"
   "~ge" means "greater than or equal to"
   "~gt" means "greater than"
   "~le" means "less than or equal to"
   "~lt" means "less than"
   "~eq" means "equal to"
   
