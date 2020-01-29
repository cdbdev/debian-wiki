# How to shutdown frozen Linux system that's not responding
| Keyboard Shortcut        | Description                                                          |
| ------------------------ |:-------------------------------------------------------------------- | 
| Alt+SysRq+r Unraw        | Take control of keyboard back from X                                 | 
| Alt+SysRq+e Terminate    | Send SIGTERM to all processes, allowing them to terminate gracefully | 
| Alt+SysRq+i Kill         | Send SIGKILL to all processes, forcing them to terminate immediately | 
| Alt+SysRq+s Sync         | Flush data to disk                                                   | 
| Alt+SysRq+u Unmount      | Unmount and remount all filesystems read-only                        | 
| Alt+SysRq+b Reboot       | Reboot                                                               | 


Explanation of keys:
- un**R**aw (take control of keyboard back from X)
- t**E**rminate (send SIGTERM to all processes, allowing them to terminate gracefully)
- k**I**ll (send SIGKILL to all processes except init, forcing them to terminate immediately)
- **S**ync (flush data to disk - Sync all mounted filesystems)
- **U**nmount (remount all filesystems read-only)
- re**B**oot (reboot the system, without unmounting partitions or syncing)

`REISUO` will do a shutdown rather than a restart.

Some ways to remember the key combination (mnemonic):
- **R**aising **E**lephants **I**s **S**o **U**tterly **B**oring
- **R**eboot **E**ven **I**f **S**ystem **U**tterly **B**roken
- or simply the word **BUSIER** read backwards
