# Remove Default Aps
This is basically the same process as in Windows 8.

## Remove All Modern Apps That Can be
Open Powershell with Administrator Permissions, and enter the following.

```powershell
Get-AppxPackage * | Remove-AppxPackage
```

## Remove Only Some Modern Apps
Copy the following Code Powershell, it removes 3D Printing, the Xbox app, the Money/Sports/News/Weather (Bing) apps, the Music and TV/Videos app, the Photos app, the Mail/Calendar app, the Solitaire app, the Phone app, the Voice Recorder app, the Camera app, the People app, and the Map app.

```powershell
Get-AppxPackage *3d* | Remove-AppxPackage
Get-AppxPackage *xbox* | Remove-AppxPackage
Get-AppxPackage *bing* | Remove-AppxPackage
Get-AppxPackage *zune* | Remove-AppxPackage
Get-AppxPackage *photo* | Remove-AppxPackage
Get-AppxPackage *communi* | Remove-AppxPackage
Get-AppxPackage *solit* | Remove-AppxPackage
Get-AppxPackage *phone* | Remove-AppxPackage
Get-AppxPackage *soundrec* | Remove-AppxPackage
Get-AppxPackage *camera* | Remove-AppxPackage
Get-AppxPackage *people* | Remove-AppxPackage
Get-AppxPackage *map* | Remove-AppxPackage
```

Source: http://www.reddit.com/r/windows/comments/3f6gsl/remove_default_apps_from_fresh_windows_10_install/

## Remove a bit more

```powershell
get-appxpackage messaging | remove-appxpackage
get-appxpackage sway | remove-appxpackage
get-appxpackage commsphone | remove-appxpackage
get-appxpackage windowsphone remove-appxpackage
get-appxpackage phone | remove-appxpackage
get-appxpackage communicationsapps | remove-appxpackage
get-appxpackage people | remove-appxpackage
get-appxpackage zunemusic | remove-appxpackage
get-appxpackage zunevideo | remove-appxpackage
get-appxpackage zune | remove-appxpackage
get-appxpackage bingfinance | remove-appxpackage
get-appxpackage bingnews | remove-appxpackage
get-appxpackage bingsports | remove-appxpackage
get-appxpackage bingweather | remove-appxpackage
get-appxpackage bing | remove-appxpackage
get-appxpackage onenote | remove-appxpackage
get-appxpackage maps | remove-appxpackage
get-appxpackage solitaire | remove-appxpackage
get-appxpackage officehub | remove-appxpackage
get-appxpackage skypeapp | remove-appxpackage
get-appxpackage getstarted | remove-appxpackage
get-appxpackage 3dbuilder | remove-appxpackage
Get-AppxPackage drawboardpdf | Remove-AppxPackage
Get-AppxPackage freshpaint | Remove-AppxPackage
Get-AppxPackage nytcrossword | Remove-AppxPackage
Get-AppxPackage microsoft.xboxapp | Remove-AppxPackage
Get-AppxPackage SurfaceHub | Remove-AppxPackage
Get-AppxPackage flipboard | Remove-AppxPackage
```

Source: https://www.reddit.com/r/pcmasterrace/comments/736tfh/skype_is_officially_bloatware_uninstalled_it/dno4ga5/