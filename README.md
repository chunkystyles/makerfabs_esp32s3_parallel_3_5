This is a project to get LVGL and Squareline Studio working on the 3.5 inch parallel TFT ESP32-S3 device made by Makerfabs: https://www.makerfabs.com/esp32-s3-parallel-tft-with-touch-ili9488.html

There is only a single touch slider in the middle of the screen provided by ui files generated by Squareline Studio.

I uploaded this to the device using VS Code, but you should also be able to use the Arduino IDE.

If you are using your own UI files generated by Squareline Studio, there were a few things I had to do to get this to compile.  The main thing was that I had to flatten the file structure and redo all of the imports.  Arduino will not compile files thare are not in the same directory as the .ino file.

I copied code from https://github.com/0015/ThatProject/blob/master/ESP32_LVGL/LVGL8_SquareLine/03_Let's_build_a_GPS_Speedometer/SC01Plus_BN880Q_GPS_App_Part2/SC01Plus_BN880Q_GPS_App_Part2.ino to get LVGL configured properly.

The "boards" folder contains a definition of the device for Squareline Studio.  See the readme file in that directory for more information.