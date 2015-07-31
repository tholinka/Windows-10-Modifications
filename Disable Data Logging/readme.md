#Disable Data Logging
This disables most data logging, and through disabling web search also makes search behave similarly to Windows 7

##Steps
There's been a lot of commotion over W10's privacy terms. I'm sure these methods can change/improve at any time, but here's a guide which should hopefully give you a relatively more private, safe experience, however at the risk of not being able to enjoy some of W10's features.

###Before/During Installation**

* Do **not** use *Express Settings*. Hit *Customize*, and make sure everything is turned off.
* It's strongly preferred that you use a **local account** with Windows 10.

###After Installation

* Head to *Settings &gt; Privacy*, and disable **everything**, unless there are some things you really need.

* While within the Privacy page, go to *Feedback*, select *Never* in the first box, and *Basic* in the second box.

* Disable Cortana by clicking the *Search* bar/icon.

* Change the name of your PC by going to Start (or hitting the Windows key), typing *About PC*, and clicking *Rename PC*.

###Slightly Complex

* Open up the *Command Prompt* by launching **cmd** as an administrator, and enter the following:

&gt; sc delete DiagTrack

&gt; sc delete dmwappushservice

&gt; echo "" &gt; C:\ProgramData\Microsoft\Diagnosis\ETLLogs\AutoLogger\AutoLogger-Diagtrack-Listener.etl

* Open up the *Group Policy Editor* by launching **gpedit.msc** as an administrator. Go through *Computer Configuration &gt; Administrative Templates &gt; Windows Components &gt; Data Collection and Preview Builds*. Double click *Telemetry*, hit *Disabled*, then apply. **NOTE: This only *truly* works in the Enterprise edition, but the final step provides a decent enough workaround for Pro users.**



* Open up the *Registry Editor* by launching **regedit** as an administrator. Go through *HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\DataCollection*, select *AllowTelemetry*, change its value to *0*, then apply.

* First, run InstallTakeOwnership.reg. Then, head to the *Hosts File* by going through *C:\Windows\System32\Drivers\Etc*, take ownership of the *hosts* file, and add all of the IPs from ips.txt

###Optional
* Disable web search in Search by going to Settings, and turning off *Search online and include web results*.

* Head to *Settings &gt; Update and Security &gt; Advanced Options &gt; Choose how updates are delivered*, and turn the first switch off.

* While still in the *Group Policy Editor*, go through *Computer Configuration &gt; Administrative Templates &gt; Windows Components &gt; OneDrive*, double click *Prevent the usage of OneDrive for file storage*, hit *Enabled*, then apply. **NOTE: This disables OneDrive**

* While still in the *Group Policy Editor*, go through *Computer Configuration &gt; Administrative Templates &gt; Windows Components &gt; Windows Defender*, double click *Turn Off Windows Defender*, hit *Enabled*, then apply. **NOTE: This disables Windows Defender

* Replace Microsoft Edge/Internet Explorer with **Firefox**, **Chromium**, or any forks/variations of them.
* Replace Windows Media Player with **VLC** or **MPC-HC**

* Replace Groove Music with **Foobar2000**, **Winamp**, or **MusicBee**.

* Replace Photos/Windows Photo Viewer with **ImageGlass**, **IrfanView** or **paint.net**.


Source: https://www.reddit.com/r/Windows10/comments/3f38ed/guide_how_to_disable_data_logging_in_w10/