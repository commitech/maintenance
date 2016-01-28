# Some checklists

## Login domain

Make sure the default login domain is NUSSTU. To do this, login with admin account. Run `gpedit.msc`. Click `Computer Configuration`, `Administrative Templates`, `System`, `Logon`. In the choices on the right, choose `Assign a default domain for logon`. There will be a new popup window. In the radio button on the left, click `Enabled` and type `nusstu` on the `Default Logon domain:` input box.

## Wallpaper Path

Note that we can't set the wallpaper just like how you set your wallpaper on personal computer. We must set the wallpaper path so that ALL users will have the same wallpaper. 
To do this, login with admin account. Run `gpedit.msc`. Click `User Configuration`, `Administrative Templates`, `Desktop`, `Desktop`. In the choices on the right, choose `Desktop Wallpaper`. There will be a new popup window. In the radio button on the left, click `Enabled` and type `C:\\Windows\commIT\wallpaper.jpg` (because that's where the wallpaper file is stored) on the `Default Logon domain:` input box, and choose `Wallpaper Style` to be `Fill`.

## Scripts

All scripts are to be done automatically using `Task Scheduler`