# windows-setup
How to set up Windows 10

## Windows
- O&O ShutUp10: https://www.oo-software.com/en/shutup10
- Windows 10 Decrapifier: https://community.spiceworks.com/scripts/show/4378-windows-10-decrapifier-18xx-19xx-2xxx
- YES _ Windows 10: Cortana deinstallieren: https://www.netzwelt.de/anleitung/180485-windows-10-cortana-deinstallierenso-gehts.html
- Cortana vollständig deinstallieren: https://praxistipps.chip.de/cortana-vollstaendig-deinstallieren-so-gehts_44689
- Windows 10 OneDrive entfernen: https://www.netzwelt.de/tutorial/163642-windows-10-so-deinstalliert-onedrive.html
- OneDrive deinstallieren: https://www.heise.de/tipps-tricks/OneDrive-deinstallieren-so-geht-s-4975944.html
- YES _ Web-Suche in Windows 10 deaktivieren (mit Gruppenrichtlinien): https://www.windowspro.de/wolfgang-sommergut/web-suche-windows-10-deaktivieren-gruppenrichtlinien
- Windows 10 - Websuche im Startmenü deaktivieren: https://www.bennetrichter.de/anleitungen/windows-10-websuche-deaktivieren/
- How to Force Uninstall Programs on Windows 10/11 Computers: https://wccftech.com/how-to/how-to-force-uninstall-programs-on-windows-10-11-computers/
- WhyNotWin11: https://github.com/rcmaehl/WhyNotWin11

## Programs
- Mozilla Firefox: https://www.mozilla.org/en-US/firefox/all/
- Mozilla Thunderbird: https://www.thunderbird.net/en-US/thunderbird/all/
- Adobe Acrobat Reader DC: https://get.adobe.com/reader/otherversions/
- PDF24 Creator: https://tools.pdf24.org/en/creator
- VLC Media Player: https://www.videolan.org/vlc/#download
- Microsoft Office: https://www.office.com/
- LibreOffice: https://www.libreoffice.org/download/download/
- Google Chrome: https://www.google.com/intl/en-US/chrome/
- Notepad++: https://notepad-plus-plus.org/downloads/
- iMazing HEIC Converter: https://imazing.com/heic/download

## System tools
- Sysinternals Process Explorer: https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer
- Sysinternals Autoruns: https://docs.microsoft.com/en-us/sysinternals/downloads/autoruns
- Greenshot: https://getgreenshot.org/downloads/ and https://github.com/greenshot/greenshot
- 7-Zip: https://www.7-zip.org/download.html

## Video telephony
- Microsoft Teams: https://www.microsoft.com/en-us/microsoft-teams/download-app
- Zoom: https://zoom.us/download
- Cisco Webex Meetings: https://www.webex.com/downloads.html

## WhyNotWin11
- Achitecture: 64bit instead of 32bit (CPU + OS)
- Boot method: UEFI instead of Legacy
- Disk partition type: GPT instead of MBR

Source:
- https://github.com/rcmaehl/WhyNotWin11

## Uninstall Cortana
- Go to the Windows Desktop by pressing `Win` + `D`
- Right click on the Windows icon in the bottom left
- Click on `Windows PowerShell (Administrator)`
- Copy the following command:

```
Get-AppxPackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage
```

- Paste it in the Windows PowerShell by pressing `Right click`
- Press Enter

If the command above does not work, try one of these commands:
```
Get-AppxPackage *Microsoft.549981C3F5F10* -AllUsers | Remove-AppxPackage -AllUsers

Get-AppxPackage *Microsoft.549981C3F5F10* -AllUsers | Remove-AppxPackage
```

## Rename a Wired Network Connection
- Press `Win` + `R`
- Enter `regedit.exe` or simply `regedit`
- Open the app as an admin, e.g. by pressing `Ctrl` + `Shift` + `Enter`
- Open this path:
```
HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\NetworkList\Profiles

Copy paste:
\
```
- The profiles are listed in the folders below

Sources:
- https://www.tecchannel.de/a/netzwerknamen-unter-windows-10-aendern,3277868
- https://www.pctipp.ch/praxis/windows/windows-10-netzwerke-umbenennen-so-gehts-2002978.html

## Other
- Snappy Driver Installer Origin: https://www.snappy-driver-installer.org/ (use with caution)
- Patch My PC (Check for outdated software): https://patchmypc.com/home-updater
- Samsung Magician Software for SSDs: https://www.samsung.com/semiconductor/minisite/ssd/download/tools/
- Portable Apps: https://portableapps.com/
