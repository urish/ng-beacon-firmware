# ng-beacon-firmware
ng-beacon firmware builds

## Firmware update instructions
1. Download the ZIP file with the latest build
2. Use a [Web Bluetooth](https://github.com/WebBluetoothCG/web-bluetooth/blob/gh-pages/implementation-status.md) supporting browser (e.g. Chrome on Android 6 or OSX)
3. Open the [Web DFU App](https://thegecko.github.io/web-bluetooth-dfu/examples/secure_dfu_web.html)
4. Switch the beacon to DFU mode
5. Load the .zip file into the Web DFU app, and press the "SELECT DEVICE" button to start the process
6. If it gets stuck / fails, try again. The process should resume from the point it stopped

You can also use the nRF Toolbox App ([Android](https://play.google.com/store/apps/details?id=no.nordicsemi.android.nrftoolbox&hl=en), [iOS](https://itunes.apple.com/us/app/nrf-toolbox/id820906058?mt=8)) for DFU.
