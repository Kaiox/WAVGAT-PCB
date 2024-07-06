# WAVGAT-PCB

This guide explains how to use the WAVGAT Arduino copy PCB, including compiling and building in the Arduino IDE, only if you don't want to use LGT8F328 (default board compiler in Arduino IDE).

## Firmware Software

- [Download from WCH](https://www.wch.cn/download/CH341SER_EXE.html)
- Local file: `CH341SER.exe`

## Arduino IDE Update

Follow the instructions inspired by this [Arduino Forum post](https://forum.arduino.cc/t/debutant-besoin-daides-carte-arduino-uno-r3-wavgat-et-module-rc522/564695/14) to update your Arduino IDE for compatibility with WAVGAT boards.

### Steps to Update

1. **Install CH341 Driver**:
   - Download the driver from the link provided above.
   - Run `CH341SER.exe` to install the driver.

2. **Configure Arduino IDE**:
   - Open the Arduino IDE.
   - Go to `File` -> `Preferences`.
   - In the `Additional Boards Manager URLs` field, add the following URL:
     ```
     http://download.wch.cn/ch341/CH341SER.zip
     ```
   - Click `OK`.

3. **Install WAVGAT Board Package**:
   - Go to `Tools` -> `Board` -> `Boards Manager`.
   - Search for "WAVGAT".
   - Install the WAVGAT board package.

4. **Select the WAVGAT Board**:
   - Go to `Tools` -> `Board`.
   - Select the appropriate WAVGAT board from the list.

5. **Upload a Sketch**:
   - Write your Arduino sketch as usual.
   - Select the correct port from `Tools` -> `Port`.
   - Click the upload button to upload your sketch to the WAVGAT board.

## Troubleshooting

If you encounter issues, refer to the [Arduino Forum post](https://forum.arduino.cc/t/debutant-besoin-daides-carte-arduino-uno-r3-wavgat-et-module-rc522/564695/14) for additional tips and solutions.

## Conclusion

By following these steps, you should be able to use your WAVGAT Arduino copy PCB with the Arduino IDE successfully.
