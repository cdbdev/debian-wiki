# How to shutdown frozen Linux system that's not responding
Holding down `Alt + SysRq` (SysRq = Print Screen key) while slowly typing `REISUB` will get you safely restarted. 

listing of all the SysRq keys:
- R: Switch the keyboard from raw mode to XLATE mode
- E: Send the SIGTERM signal to all processes except init
- I: Send the SIGKILL signal to all processes except init
- S: Sync all mounted filesystems
- U: Remount all mounted filesystems in read-only mode
- B: Immediately reboot the system, without unmounting partitions or syncing

`REISUO` will do a shutdown rather than a restart.
