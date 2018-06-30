# Building the ng-beacon firmware

Use an Ubuntu linux machine (or virtual machine). It should also be possible to build the firmware under Windows 10 Linux Subsystem.

1. Clone the firmware source code repo and checkout the ng-beacon branch:
```shell
git clone https://github.com/urish/Espruino
git checkout ng-beacon
``` 

2. Set up your build environment by running the following script:
```shell
source scripts/provision.sh NGBEACON
```

3. Run the Make command to build the bootloader:
```shell
make BOARD=NGBEACON RELEASE=1 BOOTLOADER=1 
```

4. Then the actual firmware:
```shell
make BOARD=NGBEACON RELEASE=1
``` 

5. The firmware will be built into `espruino_1vMM.NNN_ngbeacon.hex`, where MM is the major version number and NNN is the minor version number. Use a j-link programmer (or a Raspberry Pi) to flash the new firmware.

## Building a DFU update build

Follow the instructions above, but replace the command for step 4 with:
```shell
make BOARD=NGBEACON RELEASE=1 DFU_UPDATE_BUILD=1
```
