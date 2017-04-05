# ng-beacon-firmware
ng-beacon firmware builds

## Firmware update instructions
1. Download the ZIP file with the latest build
2. Extract the ZIP file, you will find a .dat and .bin file inside
3. Use a [Web Bluetooth](https://github.com/WebBluetoothCG/web-bluetooth/blob/gh-pages/implementation-status.md) supporting browser (e.g. Chrome on Android 6 or OSX) and open the [Web DFU App](https://urish.github.io/web-bluetooth-secure-dfu)
4. Switch the beacon to DFU mode
5. Load the .dat and .bin file into the Web DFU app, and press the DFU button to start the process.
6. If it gets stuck / fails, try again. It should work on the 2nd or 3rd try.

You can also use the nRF Toolbox App ([Android](https://play.google.com/store/apps/details?id=no.nordicsemi.android.nrftoolbox&hl=en), [iOS](https://itunes.apple.com/us/app/nrf-toolbox/id820906058?mt=8)) for DFU.
