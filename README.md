# windows-setup
How to set up Windows 10.

Useful information, tips & tricks and other relevant resources to properly configure a Windows 10 user account/ computer.

Note: Some content is focused on Germany.

## Programs
- Mozilla Firefox: https://www.mozilla.org/en-US/firefox/all/
- Google Chrome: https://www.google.com/intl/en-US/chrome/
- Mozilla Thunderbird: https://www.thunderbird.net/en-US/thunderbird/all/
- Adobe Acrobat Reader DC: https://get.adobe.com/reader/otherversions/
- PDF24 Creator: https://tools.pdf24.org/en/creator
- Notepad++: https://notepad-plus-plus.org/downloads/
- Microsoft Office: https://www.office.com/
- LibreOffice: https://www.libreoffice.org/download/download/
- VLC Media Player: https://www.videolan.org/vlc/#download
- iMazing HEIC Converter: https://imazing.com/heic/download

## System tools
- Sysinternals Process Explorer: https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer
- Sysinternals Autoruns: https://docs.microsoft.com/en-us/sysinternals/downloads/autoruns
- Greenshot: https://getgreenshot.org/downloads/ and https://github.com/greenshot/greenshot
- 7-Zip: https://www.7-zip.org/download.html
- WinDirStat Portable: https://portableapps.com/de/apps/utilities/windirstat_portable

## Video telephony
- Microsoft Teams: https://www.microsoft.com/en-us/microsoft-teams/download-app
- Zoom: https://zoom.us/download
- Cisco Webex Meetings: https://www.webex.com/downloads.html
- Teamviewer: https://www.teamviewer.com/download/windows
- Teamviewer German: https://www.teamviewer.com/de/download/windows
- Linphone: https://www.linphone.org

## Remove Adware and Potentially Unwanted Programs
- AdwCleaner: https://www.malwarebytes.com/adwcleaner

## Other 1
- O&O ShutUp10 https://www.oo-software.com/en/shutup10
- Windows 10 Decrapifier https://community.spiceworks.com/scripts/show/4378-windows-10-decrapifier-18xx-19xx-2xxx
- YES _ Windows 10: Cortana deinstallieren https://www.netzwelt.de/anleitung/180485-windows-10-cortana-deinstallierenso-gehts.html
- Cortana vollständig deinstallieren https://praxistipps.chip.de/cortana-vollstaendig-deinstallieren-so-gehts_44689
- Windows 10 OneDrive entfernen https://www.netzwelt.de/tutorial/163642-windows-10-so-deinstalliert-onedrive.html
- OneDrive deinstallieren https://www.heise.de/tipps-tricks/OneDrive-deinstallieren-so-geht-s-4975944.html
- YES _ Web-Suche in Windows 10 deaktivieren (mit Gruppenrichtlinien) https://www.windowspro.de/wolfgang-sommergut/web-suche-windows-10-deaktivieren-gruppenrichtlinien
- Windows 10 - Websuche im Startmenü deaktivieren https://www.bennetrichter.de/anleitungen/windows-10-websuche-deaktivieren/
- How to Force Uninstall Programs on Windows 10/11 Computers https://wccftech.com/how-to/how-to-force-uninstall-programs-on-windows-10-11-computers/
- Windows 10 installieren 2022 - Mit USB + Einrichten & Treiber Installation, HardwareDealz https://www.youtube.com/watch?v=G5TGARdHkRM 
- Systemfehler mit SFC und DISM reparieren (`sfc /scannow`) https://www.netzwelt.de/anleitung/166183-windows-10-so-behebt-fehler-ueber-sfc-dism.html
- https://www.makeuseof.com/difference-between-chkdsk-sfc-and-dism-in-windows-10/
- https://superuser.com/questions/1658332/run-sfc-scannow-or-chkdsk-f-first
- https://superuser.com/questions/1579030/what-is-the-purpose-of-the-dism-restorehealth-parameter-and-sfc
- https://superuser.com/questions/1330365/how-will-dism-online-cleanup-image-restorehealth-affect-my-current-configurat
- Deactivate Internet Explorer https://docs.microsoft.com/en-us/troubleshoot/developer/browsers/installation/disable-internet-explorer-windows

## Other 2
- Snappy Driver Installer Origin: https://www.snappy-driver-installer.org/ (use with caution)
- Patch My PC (Check for outdated software): https://patchmypc.com/home-updater
- Samsung Magician Software for SSDs: https://www.samsung.com/semiconductor/minisite/ssd/download/tools/
- Portable Apps: https://portableapps.com/
- CPU-Z: https://en.wikipedia.org/wiki/CPU-Z

## Remove or Uninstall Programs
If a programm cannot be uninstalled successfully through the standard procedures, this program might help
- Revo Uninstaller Free: https://www.revouninstaller.com/revo-uninstaller-free-download/

## Network Scanner
- Advanced IP Scanner: https://www.advanced-ip-scanner.com
- Angry IP Scanner: https://angryip.org

## WhyNotWin11
- Achitecture: `64bit` instead of `32bit` (both CPU and OS)
- Boot method: `UEFI` instead of `Legacy`
- Disk partition type: `GPT` instead of `MBR`

Source:
- https://github.com/rcmaehl/WhyNotWin11
- Download WhyNotWin11 latest stable release (64-bit): https://github.com/rcmaehl/WhyNotWin11/releases/latest/download/WhyNotWin11.exe

## Microsoft account
- https://account.microsoft.com Microsoft account overview
- https://account.microsoft.com/devices Devices linked to Microsoft account
- https://account.microsoft.com/services/microsoft365/install Devices logged in to Microsoft 365
- https://account.microsoft.com/devices/content Devices linked to the Microsoft Store

## Uninstall Cortana
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
```
- The profiles are listed in the folders below

Sources:
- https://www.tecchannel.de/a/netzwerknamen-unter-windows-10-aendern,3277868
- https://www.pctipp.ch/praxis/windows/windows-10-netzwerke-umbenennen-so-gehts-2002978.html

## Change hostname
- Press the `Windows` key in the bottom left
- Search for `PC Info`
- Click on `Rename this PC`

Sources:
- https://support.microsoft.com/en-us/windows/rename-your-windows-10-pc-750bc75d-8ff8-e99a-b9dc-04dff566ae74

## Password of SMB fileshares
- Press `Win` + `R`
- Enter `netplwiz.exe`

## Remove Web Results from Windows Search
- Suche: `Gruppenrichtlinien bearbeiten` / `gpedit.msc`
- `Administrative Vorlagen`
- `Windows-Komponenten`
- `Suche`
- `Nicht im Web suchen und keine Webergebnisse in der Suche anzeigen`

## Disable Bing in the Start Menu Search
- https://www.howtogeek.com/224159/how-to-disable-bing-in-the-windows-10-start-menu/

## Disable OneDrive Synchronization
- https://www.cbackup.com/articles/stop-onedrive-from-syncing-6688.html
- https://www.minitool.com/backup-tips/how-to-disable-onedrive.html
- https://helpdeskgeek.com/windows-10/how-to-disable-onedrive-on-your-windows-10-pc-why-youd-want-to/

## Useful Windows applications
- `winver.exe` About Windows / Windows-Version
- `msinfo32.exe` System Information / Systeminformationen
- `devmgmt.msc` Device Manager / Geräte-Manager
- `diskmgmt.msc` Disk Management / Datenträgerverwaltung
- `dfrgui.exe` Optimize Drives / Laufwerke defragmentieren und optimieren
- `perfmon.exe` Resource Monitor / Ressourcenmonitor
- `regedit.exe` Registry Editor / Registrierungs-Editor
- `netplwiz.exe` User Accounts / Benutzerkontenverwaltung
- `compmgmt.msc` Computer Management / Computerverwaltung
- `cleanmgr.exe` Disk Cleanup / Datenträgerbereinigung
- `msconfig.exe` System Configuration / Systemkonfiguration
- `SystemPropertiesProtection.exe` System Protection / Computerschutzeinstellungen
- PC Health Check / PC-Integritätsprüfung

## Nasty Networking Issue
- https://social.technet.microsoft.com/Forums/windows/de-DE/17c9ea7d-52df-4ef9-95fa-0a961d11bfa3/fix-for-cannot-access-nas-drives-sharefolder-is-not-accessible-or-quoterror-code
- https://www.stellarinfo.co.in/blog/how-to-fix-nas-device-not-visible-on-windows-10/
- https://kb.synology.com/en-nz/DSM/tutorial/What_can_I_do_if_my_Synology_NAS_does_not_show_up_in_Network_in_Windows_File_Explorer
- https://www.buffalotech.com/knowledge-base/windows-10-cannot-access-shares-on-nas
- https://www.google.de/search?q=%220x80070035%22
- https://basic-tutorials.de/ratgeber/software/fehlerbehebung-0x80070035-fehlercode-der-netzwerkpfad-wurde-nicht-gefunden/
- https://de.minitool.com/nachrichten/der-netzwerkpfad-wurde-nicht-gefunden.html
- https://hdwh.de/windows-10-netzwerk-zeigt-fehler-0x80070035-der-netzwerkpfad-wurde-nicht-gefunden/
- https://www.borncity.com/blog/2015/09/21/windows-10-netzwerk-zeigt-fehler-0x80070035/
- https://www.expertiger.de/windows-problem/windows-fehler-0x80070035
- https://www.windows-faq.de/2018/02/22/0x80070035-fehlercode-der-netzwerkpfad-wurde-nicht-gefunden/
- https://www.youtube.com/watch?v=5bIcJluf-0Q Network Path Not Found - WIndows 10 1803 - Guaranteed Fix
- https://docs.microsoft.com/en-us/troubleshoot/windows-client/networking/cannot-access-shared-folder-file-explorer
- https://docs.microsoft.com/en-us/troubleshoot/windows-client/networking/mapped-drives-not-available-from-elevated-command
- https://docs.qnap.com/operating-system/qts/5.0.x/de-de/webserver-091B47DC.html
- https://forum.qnapclub.de/thread/58177-keine-verbindung-%C3%BCber-browser/

Problem:
- Windows 10 error code 0x80070035
- When trying to open a network share, Windows 10 does not show a prompt to enter the username and password

Solution:
- Enter the NAS hostname, username and password manually via `netplwiz`

Question:
- Why does Windows 10 not show the prompt to enter the username and password for a network share? Maybe it is related to the user permissions or rights?
