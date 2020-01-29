# How to shutdown frozen Linux system that's not responding
There are several low level shortcuts that are implemented in the kernel which can be used for debugging and recovering from an unresponsive system. Whenever possible, it is recommended that you use these shortcuts instead of doing a hard shutdown (holding down the power button to completely power off the system). 

A common used method is: `REISUB`:

| Keyboard Shortcut        | Description                                                          |
| ------------------------ |:-------------------------------------------------------------------- | 
| `Alt+SysRq+r` Unraw        | Take control of keyboard back from X                                 | 
| `Alt+SysRq+e` Terminate    | Send SIGTERM to all processes, allowing them to terminate gracefully | 
| `Alt+SysRq+i` Kill         | Send SIGKILL to all processes, forcing them to terminate immediately | 
| `Alt+SysRq+s` Sync         | Flush data to disk                                                   | 
| `Alt+SysRq+u` Unmount      | Unmount and remount all filesystems read-only                        | 
| `Alt+SysRq+b` Reboot       | Reboot                                                               | 

> **REMARK:** `REISUO` will do a shutdown rather than a restart.

Some ways to remember the key combination (mnemonic):
- **R**aising **E**lephants **I**s **S**o **U**tterly **B**oring
- **R**eboot **E**ven **I**f **S**ystem **U**tterly **B**roken
- or simply the word **BUSIER** read backwards
