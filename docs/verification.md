Now that we have successfully flashed the firmware, let's verify the version number. In the serial terminal, send the command `VERSIONA`. The UM980 will respond by providing the firmware version and authorization date. Look for the part of the message after the model number (i.e. "UM980"). This should match the build number from **&#42;pkg** file name.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_Firmware_Verification.JPG"><img src="../assets/img/UPrecise_Software_Firmware_Verification.JPG" width="600px" height="600px" alt="UPrecise Software: Sending Command VERSIONA"></a></td>
    </tr>
  </table>
</div>

!!! note
    Sending the command `VERSIONA` is one method of verifying the version number on the UM980. You can use the [Arduino example code](https://docs.sparkfun.com/SparkFun_UM980_Triband_GNSS_RTK_Breakout/arduino_examples/#example-15-query-device) to verify the version number on the UM980 breakout board.

    <div style="text-align: center;">
      <table>
        <tr style="vertical-align:middle;">
         <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/Arduino_Output_Ex_15_ESP32_Triband_GNSS_RTK_UM980_Highlighted.JPG"><img src="../assets/img/Arduino_Output_Ex_15_ESP32_Triband_GNSS_RTK_UM980_Highlighted.JPG" width="600px" height="600px" alt="UM980 Firmware Output with Arduino"></a></td>
        </tr>
      </table>
    </div>

Try viewing the UM980 output through the UPrecise software. Not seeing any satellites in the GUI or output in the serial terminal? Try adjusting the configuration to output every second. From the menu, head to the following to configure the messages: **Receiver Configurations** > **Message configuration**. In this case, we selected the following: **GGA**, **GSA**, **GSV**, **RMC**, **GST**. Feel free to select more depending on your application.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_Receiver_Configurations.JPG"><img src="../assets/img/UPrecise_Software_Receiver_Configurations.JPG" width="600px" height="600px" alt="UPrecise Software: Receiver Configurations - Message configuration"></a></td>
    </tr>
  </table>
</div>



Scroll down **Receiver Configurations** window and select **Enter** button.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_Receiver_Configurations_Send.JPG"><img src="../assets/img/UPrecise_Software_Receiver_Configurations_Send.JPG" width="600px" height="600px" alt="UPrecise Software: Receiver Configurations - Message configuration, Enter"></a></td>
    </tr>
  </table>
</div>

You should be able to see messages outputting through the serial terminal and displaying graphically.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_UM980_Connected_Quality_Single_Point_Positioning.JPG"><img src="../assets/img/UPrecise_Software_UM980_Connected_Quality_Single_Point_Positioning.JPG" width="600px" height="600px" alt="UPrecise Software with UM980 Outputting Messages with Data Single Point Positioning"></a></td>
    </tr>
  </table>
</div>
