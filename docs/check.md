# Some checklists

## Login domain

Make sure the default login domain is NUSSTU. To do this, login with admin account. Run "gpedit.msc". Click "Computer Configuration", "Administrative Templates", "System", "Logon". In the choices on the right, choose "Assign a default domain for logon". There will be a new popup window. In the radio button on the left, click "Enabled" and type "nusstu" on the "Default Logon domain:" input box.

## Wallpaper Path

Note that we can't set the wallpaper just like how you set your wallpaper on personal computer. We must set the wallpaper path so that ALL users will have the same wallpaper. 
To do this, login with admin account. Run "gpedit.msc". Click "User Configuration", "Administrative Templates", "Desktop", "Desktop". In the choices on the right, choose "Desktop Wallpaper". There will be a new popup window. In the radio button on the left, click "Enabled" and type "C:\\Windows\commIT\wallpaper.jpg" (because that's where the wallpaper file is stored) on the "Default Logon domain:" input box, and choose "Wallpaper Style" to be "Fill".

## Scripts

All scripts are to be done automatically using "Task Scheduler".

### YIH

These are the scripts that has to be installed :

- Delprof2_Scheduler
- printer_installer
- shutdown_weekdays_yih
- shutdown_saturday_yih
- shutdown_sunday_yih
- shutdown_message_weekdays_yih
- shutdown_message_saturday_yih
- shutdown_message_sunday_yih
- wallpaper_download

The scripts are in the form of .xml file so that Task Scheduler can read it. The scripts can be taken from supervisor-2 PC, which is `\\YI-1-51K0T92\commIT`

### CL
These are the scripts that has to be installed :

- Delprof2_Scheduler
- printer_installer
- wallpaper_download
TBA

To install the script, login using admin account and open "Task Scheduler". Click "Task Scheduler Library". Without choosing any script, click "Action" at the menu bar and click "Import Task". Browse the script that you would like to add. 

After that, a new window will appear. Click "Change User or Group" button. In the "Enter the object name to select" text area, enter the admin account of the computer (i.e. "unotadmin" for CL and "PCADMINYIH" for YIH). Choose the "Run whether user is logged on or not" radio button. Click "OK". You may prompted to enter the admin account, so enter it and click OK.

## Auto update

We want to change the automatic updates settings from the default. To do this, login with admin account. Run "gpedit.msc". Click "Computer Configuration", "Administrative Templates", "Windows Components", "Windows Update". In the choices on the right, choose "Configure Automatic Updates". There will be a new popup window. In the radio button on the left, click "Enabled" and choose the 2nd option "Notify for download and notify for install" in the "Configure automatic updating" option. Click OK.



