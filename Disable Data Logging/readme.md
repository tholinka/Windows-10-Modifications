# Use [DisableWinTracking (see submodule)](https://github.com/10se1ucgo/DisableWinTracking)
DisableWinTracking does most of what this document used to, see readme-manual.md for the full list.

Things DisableWinTracking doesn't do:

# Before/During Installation
* Do not use Express Settings. Hit Customize, and make sure everything is turned off.
* It's strongly preferred that you use a local account with Windows 10.

# After Installation
* Head to Settings > Privacy, and disable everything, unless there are some things you really need.
  * Note: on the "creators" update, do not disable ```Background apps``` as this breaks search, you can however disable all apps on the list
* While within the Privacy page, go to Feedback, select Never in the first box, and Basic in the second box.
* Disable Cortana by clicking the Search bar/icon.
* Change the name of your PC by going to Start (or hitting the Windows key), typing About PC, and clicking Rename PC.

# Optional
* <sup><sup>[(credit)](https://superuser.com/a/1196624)</sup></sup> Disable web search by opening ```Local Group Policy Editor```, go to the policies at ```Computer Configuration → Administrative Templates → Windows Components → Search```
  * Set ```Allow Cortana``` to **Disable**
  * Set ```Do not allow web search``` to **Enabled**
  * Set ```Don't search the web or display web results in Search``` to **Enabled**
  * Click apply
* Replace default apps, e.g. ```Edge``` with ```Chrome```, ```Windows Media Player``` with VLC, ```Groove``` with ```Foobar2000```
