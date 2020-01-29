# How to shutdown frozen Linux system that's not responding
Holding down `Alt + SysRq` (SysRq = Print Screen key) while slowly typing `REISUB` will get you safely restarted. 

Explanation of keys:
- un**R**aw (take control of keyboard back from X)
- t**E**rminate (send SIGTERM to all processes, allowing them to terminate gracefully)
- k**I**ll (send SIGKILL to all processes except init, forcing them to terminate immediately)
- **S**ync (flush data to disk - Sync all mounted filesystems)
- **U**nmount (remount all filesystems read-only)
- re**B*oot (reboot the system, without unmounting partitions or syncing)

`REISUO` will do a shutdown rather than a restart.

Some ways to remember the key combination (mnemonic):
- **R**aising **E**lephants **I**s **S**o **U**tterly **B**oring
- **R**eboot **E**ven **I**f **S**ystem **U**tterly **B**roken
- or simply the word **BUSIER** read backwards
