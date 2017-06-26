# Building the ng-beacon firmware

Use an Ubuntu linux machine (or virtual machine). It should also be possible to build the firmware under Windows 10 Linux Subsystem.

1. Clone the firmware source code repo and checkout the ng-beacon branch:

    git clone https://github.com/urish/Espruino
    git checkout ng-beacon
    
2. Set up your build environment by running the following script:

    source scripts/provision.sh NGBEACON
 
3. Run the Make command to build the bootloader:

    make BOARD=NGBEACON RELEASE=1 BOOTLOADER=1 
  
4. Then the actual firmware:

    make BOARD=NGBEACON RELEASE=1
    
5. The firmware will be built into `espruino_1v92.NNN_ngbeacon.hex`, where NNN is the minor version number. Use a j-link programmer (or a Raspberry Pi) to flash the new firmware.
