SparkFun Triband GNSS RTK Breakout - UM980
===========================================================

[![SparkFun Triband GNSS RTK Breakout - UM980](https://cdn.sparkfun.com/r/600-600/assets/parts/2/3/4/8/1/23286-UM980-Triband-GNSS-Breakout-Feature.jpg)](https://www.sparkfun.com/products/23286)

[*SparkFun Triband GNSS RTK Breakout - UM980 (GPS-23286)*](https://www.sparkfun.com/products/23286)

The SparkFun Triband GNSS RTK Breakout features the UM980 GNSS high precision RTK position module from Unicore Communications. The UM980 is a 1408-Channel GNSS Receiver based on the Nebulas IV™ that is able to simultaneously track GPS L1/L2/L5, GLONASS L1/L2, Galileo E1/E5a/E5b/E6, Beidou B1I/B2I/B3I/B1C/B2a/B2b, QZSS L1/L2/L5, and SBAS. With this board, you will be able to know where your (or any object's) X, Y, and Z location is within roughly the width of your fingernail. When an RTK solution is reached, the module can achieve a horizontal accuracy of about 8mm (~0.3 inches) and vertical accuracy of 15mm (~0.59 inches). The UM980 is capable of both rover and base station operations.

We've included a rechargeable backup battery to keep the latest module configuration and satellite data available. This battery helps 'warm-start' the module, decreasing the time-to-first-fix dramatically. This module features a survey-in mode, allowing the module to become a base station and produce RTCM 3.x correction data. A SMA connector is included for a secure connection to a Triband GNSS antenna.

Currently, serial UART is only supported on the UM980 module. All three serial UART ports have been broken out to the USB-C connector via CH340, 4-pin locking JST connector, and BlueSMiRF header. Unique pins have also been broken out to the edge of the board. Various jumpers are also included to configure power and LEDs.



Repository Contents
-------------------

* **.github/workflows** - YAML files used for GitHub Actions and GitHub Pages/mkdocs
* **/Firmware** - UM980 Firmware packages
* **/Documents** - Datasheets and various documents related to the UM980
* **/Hardware** - Eagle files
* **/Software** - Related software for the UM980
* **/docs** - Online documentation files
  * **/assets** - Folder containing all the file assets used for product documentation
    * **/board_files** - Copy of design files used for product documentation
    * **/component_documentation** - Datasheets and manuals for hardware components
    * **/img** - Images for product documentation
  * **/github** - Files stating how to contribute and filing issues used for product documentation
  * **/javascript** - Folder containing custom javascript used for product documentation
  * **/stylesheet** - Folder containing CSS files used for product documentation
* **/overrides** - Customization files used for product documentation
  * **/.icons** - Icons used for GitHub used for product documentation
  * **./partials** - Used for product documentation



Documentation
--------------

* **[Installing an Arduino Library Guide](https://learn.sparkfun.com/tutorials/installing-an-arduino-library)** - Basic information on how to install an Arduino library.
* **[Library](https://github.com/sparkfun/SparkFun_Unicore_GNSS_Arduino_Library/)** - Unicore GNSS Arduino Library
* **[Hookup Guide](https://docs.sparkfun.com/SparkFun_UM980_Triband_GNSS_RTK_Breakout/)** - Hookup guide for the SparkFun Triband GNSS RTK Breakout - UM980.
* **[https://docs.sparkfun.com/Update_Firmware_Unicore_GNSS_Receiver/](https://docs.sparkfun.com/Update_Firmware_Unicore_GNSS_Receiver/introduction/)** - Tutorial on how to update firmware on a Unicore GNSS Receiver. This is a general tutorial that covers the RTK Torch and UM980 breakout. Note that this information also included in the SparkFun Triband GNSS RTK Breakout - UM980 Hookup Guide.



License Information
-------------------

This product is _**open source**_! 

Various bits of the code have different licenses applied. Anything SparkFun wrote is beerware; if you see me (or any other SparkFun employee) at the local, and you've found our code helpful, please buy us a round!

Please use, reuse, and modify these files as you see fit. Please maintain attribution to SparkFun Electronics and release anything derivative under the same license.

Distributed as-is; no warranty is given.

- Your friends at SparkFun.
