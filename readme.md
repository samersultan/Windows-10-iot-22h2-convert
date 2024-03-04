```
dism.exe /Export-Image /SourceImageFile:C:\Temp\Windows10_22H2\sources\install.esd /SourceIndex:3 /DestinationImageFile:C:\Temp\Windows10_22H2\sources\install.wim /Compress:max /CheckIntegrity
```


More details:


https://old.reddit.com/r/sysadmin/comments/148dw5y/where_is_the_windows_22h2_enterprise_engb_iso/

Run it when logged in with a local admin account (it's hard coded with this requirement which is a bit of a pain)

```
MediaCreationTool22H2.exe /Eula Accept /Retail /MediaLangCode en-GB /MediaArch x64 /MediaEdition Enterprise
```

You could then convert the esd to wim if you're so inclined.

```
dism.exe /Export-Image /SourceImageFile:C:\Temp\Windows10_22H2\sources\install.esd /SourceIndex:3 /DestinationImageFile:C:\Temp\Windows10_22H2\sources\install.wim /Compress:max /CheckIntegrity
```


----

If updating from Windows Update Fails try the followng article:

https://learn.microsoft.com/en-us/microsoftteams/troubleshoot/teams-rooms-and-devices/teams-rooms-device-windows-update-issues


---

Alt try windows 11 update:

https://m365community.blogspot.com/2023/05/windows-11-support-for-teams-rooms-on.html
