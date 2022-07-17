# x86pc
TurboDOS drivers for an x86 based PC

These files are from my testing environment for QEMNU VM-based TurboDOS x86 with a serial console and testing with the x86-based PC with a serial console.

More cleanup work will be required.  

The UARTI86 drivers are here for testing on various PC-based serial chips and make a universal driver based on a 16650-like serial controller chip to support a high-speed console or CKTSER network connection.  

Drivers for Hard Disk and Floppy disk boot sectors for boot the system,  and HD driver that requires setting up the correct parameter blocks based on the hard disk size.  Uses the ROM BIOS to call all HD and Floppy read/writes.  

An IDLE routine called by a new DSPCHR to idle the processor when running as guest OS by QEMU so that the CPU does not run at 100% all the time.
