#Remove Default Aps
This is basically the same process as in Windows 8.

##Remove All Modern Apps That Can be
Open Powershell with Administrator Permissions, and run the follow code.

Get-AppxPackage * | Remove-AppxPackage

##Remove Only Some Modern Apps
Copy the following Code Powershell, it removes 3D Printing, the Xbox app, the Money/Sports/News/Weather (Bing) apps, the Music and TV/Videos app, the Photos app, the Mail/Calendar app, the Solitaire app, the Phone app, the Voice Recorder app, the Camera app, the People app, and the Map app.

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

Source: http://www.reddit.com/r/windows/comments/3f6gsl/remove_default_apps_from_fresh_windows_10_install/