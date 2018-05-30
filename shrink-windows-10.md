[Complete Instructions Here](https://www.download3k.com/articles/How-to-shrink-a-disk-volume-beyond-the-point-where-any-unmovable-files-are-located-00432)

There are 3 steps:

1. Open Windows Powershell as an admin (right-click and select run as administrator.

Disable Hibernation so the space can be reclaimed
Run:
```powercfg /h off```

2. Disable Pagefile

```Step 1: Press Win+R (or Win+S), enter SystemPropertiesPerformance.exe, press Enter. Click the Advanced tab.

Step 2: Click Change under Virtual Memory and uncheck Automatically manage paging file size for all drives.

Step 3: Click on the partition you are trying to resize and set paging file size to No paging file. Click Set, then Ok.
```



3. Disable System Protection
This will disable restore points and delete your old restore points!
```Go to 'System Properties' and select the 'System Protection' tab.
Under 'Protection Settings' select the drive you want to partition and select 'Configure'
Select 'Disable system protection'```

At this point the resizing should work but you also may need to restart. I didn't need to I don't think but your mileage may vary.

After you resize your partition you'll likely want to reverse the steps taken above. I didn't feel it necessary as Windows is not my main OS. If you wish to reverse the changes, view the link at the top of this how-to.
