# Linux-CPU-Performance-Toggle
This repository provides scripts for AMD and Intel CPUs to toggle setting the CPUs to use up to their base clock frequencies. There are instructions to automatically apply the change when the computer starts.

This was tested with Linux Mint 21.2 Cinnamon x64 but it could work well with other distros.

For AMD CPUs:

AMD CPU Performance Toggle Information

This was tested on an AMD Ryzen 5 5600H.

Open a command-line window and enter the following:

sudo nano /etc/rc.local

#!/bin/sh -e

sh '/home/%USERNAME%/.local/bin/AMD_CPU_Performance_Toggle.sh'

Press "Crtl+X", "Y", and "Enter" to save and exit.

Place the script into the following directory:

/home/%USERNAME%/.local/bin/AMD_CPU_Performance_Toggle.sh

Enter the following commands:

sudo chown root /etc/rc.local

sudo chmod 755 /etc/rc.local

sudo /etc/rc.local start

For Intel CPUs:

Intel CPU Performance Toggle Information

This was tested on an Intel Core i5-7300HQ.

Open a command-line window and enter the following:

sudo nano /etc/rc.local

#!/bin/sh -e

sh '/home/%USERNAME%/.local/bin/Intel_CPU_Performance_Toggle.sh'

Press "Crtl+X", "Y", and "Enter" to save and exit.

Place the script into the following directory:

/home/%USERNAME%/.local/bin/Intel_CPU_Performance_Toggle.sh

Enter the following commands:

sudo chown root /etc/rc.local

sudo chmod 755 /etc/rc.local

sudo /etc/rc.local start
