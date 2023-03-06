# Core-Windows-Processes
Core Windows Processes Under develop

## Windows process explorer tools

+ Task Manage ( GUI )
+ Process Hacker ( GUI )
+ tasklist ( CLI )
+ Get-Process ( CLI )
+ ps  ( CLI )


-----------------------------------------
###  System process :
special kind of process that hosts threads that only run only in kernel-mode executing code loaded in system space.
| Process Name  | System |
| ------------- | ------------- |
| PID | 4 |
| Parent Process | None |
|  Child Processes | smss.exe |
| Image Path  | C:\Windows\system32\ntoskrnl.exe |
| Start Time | At boot time |
| User | NT AUTHORITY\SYSTEM |
| Unusual behaviour  | - parent process is different <br> - Multiple instances of System <br> - Different PID <BR> - Not running in Session 0|
-----------------------------------------

  
### Smss process :   
+ Known as the Windows Session Manager
+ Starts the kernel and user modes of the Windows subsystem
+ Responsible for creating new sessions
+ Responsible for creating environment variable
+ Virtual memory paging files
  
| Process Name  | System |
| ------------- | ------------- |
| PID | Random |
| Parent Process | System |
| Child Processes | SMSS.EXE (Session 0) for OS <br> SMSS.EXE (Session 1) for User <br> AUTOCHK.EXE and a new SMSS.EXE instance for each new session |
| Image Path  |C:\Windows\System32\smss.exe |
| Start Time | Within seconds of boot time for the master instance |
| User | NT AUTHORITY\SYSTEM |
| Number of Instances | One master instance and child instance per session <br> The child instance exits after creating the session. |
| Unusual behaviour  | Different parent process <br> - Different image path <br> - Different runing user <br> - Unexpected registry entries for Subsystem <br> - More than one running process  |
-----------------------------------------
  
  
  ### csrss process :
  +
  +
  +
  +
  +
  
  
  

| Process Name  | System |
| ------------- | ------------- |
| PID | 4 |
| Parent Process | None |
|  Child Processes | smss.exe |
| Image Path  | C:\Windows\system32\ntoskrnl.exe |
| Start Time | At boot time |
| User | NT AUTHORITY\SYSTEM |
| Number of Instances | 1 |
| unusual behaviour  | test <br> test2 |




  









<br>
System
System > smss.exe
csrss.exe
wininit.exe
wininit.exe > services.exe
wininit.exe > services.exe > svchost.exe
lsass.exe
winlogon.exe
explorer.exe
