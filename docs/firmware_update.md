!!! note
     The following instructions were taken from the UPrecise User Manual: 2.2.11 Receiver Upgrade. For more information about how to use UPrecise software, make sure to check out the user manual.

!!! note
    At the time of writing, UPrecise Version 2.0 was used. Note that the GUI appearance and features may change upon future releases.

You can update your firmware (they call this a firmware upgrade in the manual) using Unicore's UPrecise software. Make sure to check [Unicore's UM980 product page](https://en.unicorecomm.com/products/detail/26), [download center](https://en.unicorecomm.com/download), or contact Unicore Communications for any firmware releases.

We'll assume that you have the firmware downloaded at this point and connected to the UM980. With UPrecise open, click on the menu with the triple bar (**&equiv;**) near the upper left of the window to expand the menu.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_COM_Port_Connected.JPG"><img src="../assets/img/UPrecise_Software_COM_Port_Connected.JPG" width="600px" height="600px" alt="UPrecise Software: COM Port Connected"></a></td>
    </tr>
  </table>
</div>

The menu should expand with text next to each icon.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_Expand_Menu_Connected.JPG"><img src="../assets/img/UPrecise_Software_Expand_Menu_Connected.JPG" width="600px" height="600px" alt="UPrecise Software: Menu Expanded"></a></td>
    </tr>
  </table>
</div>

Click on the **Receiver Upgrade** button. The following window should open up.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_Receiver_Upgrade.JPG"><img src="../assets/img/UPrecise_Software_Receiver_Upgrade.JPG" width="600px" height="600px" alt="UPrecise Software: Receiver Upgrade"></a></td>
    </tr>
  </table>
</div>

Click the **Select upgrade file** button. Head to the folder where you downloaded the firmware and select the file. The extension should be a  **&#42;pkg** file.  In this case, there was a copy of the firmware in the [GitHub SparkFun UM980 Triband GNSS RTK Breakout Repo](https://github.com/sparkfun/SparkFun_UM980_Triband_GNSS_RTK_Breakout/tree/main/Firmware) named "_UM980_R4.10Build11833.pkg_". Older firmware versions were moved to the **Old Firmware** folder.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_Select_File.JPG"><img src="../assets/img/UPrecise_Software_Select_File.JPG" width="600px" height="600px" alt="UPrecise Software: Select File"></a></td>
    </tr>
  </table>
</div>

<!--

NO OPTION FOR DOUBLE BACKUP...

If necessary, you can select the "Double backup" checkbox. Once the module has finished updating, the main partition makes a backup in the backup partition. If the main partition fails, the module will boot from the backup partition.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/"><img src="../assets/img/" width="600px" height="600px" alt=""></a></td>
    </tr>
  </table>
</div>

-->

Select the GNSS receiver that will be receiving the firmware update. In this case it was **Receiver1**. While we are at it, select either the "**Soft reset**" or "**Hard reset**". While updating, the module will need to be reset and this selection will determine the reset method. Let's select the "**Soft Reset**" and have UPrecise reset the module.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_Select_Receiver_Reset_Method.JPG"><img src="../assets/img/UPrecise_Software_Select_Receiver_Reset_Method.JPG" width="600px" height="600px" alt="UPrecise Software: Select Receiver and Reset Method"></a></td>
    </tr>
  </table>
</div>

When ready, hit the "Start" button!

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_Firmware_Updating_Soft_Reset.JPG"><img src="../assets/img/UPrecise_Software_Firmware_Updating_Soft_Reset.JPG" width="600px" height="600px" alt="UPrecise Software: Firmware Update in Progress with Soft Reset Method"></a></td>
    </tr>
  </table>
</div>

!!! warning
    Make sure to pay attention to the progress bar! You'll want to avoid any interruptions while the firmware is updating as this will cause the upgrade to fail.

!!! note
    If you have issues updating the software with the reset method chosen, try exiting the Receiver Upgrade menu by hitting the "x" button. Then disconnect and reconnect the module by selecting the "Connect" button. You will then need to open the **Receiver Upgrade** window again before hitting the "Start" button.

Once the firmware has been updated, you will notice that the progress bar is at 100% and a message indicating that the firmware upgrade is finished. You can exit out of the window by clicking on the "**x**" button.

<div style="text-align: center;">
  <table>
    <tr style="vertical-align:middle;">
     <td style="text-align: center; vertical-align: middle;"><a href="../assets/img/UPrecise_Software_Receiver_Upgrade_Finished.JPG"><img src="../assets/img/UPrecise_Software_Receiver_Upgrade_Finished.JPG" width="600px" height="600px" alt="UPrecise Software: Receiver Upgrade Finished"></a></td>
    </tr>
  </table>
</div>

Upon exiting, you can continue viewing the UM980 output through the UPrecise software.

Not seeing any satellites or output in the serial terminal? Try adjusting the configuraiton. From the menu, head to the following to configure the messages: **Receiver Configurations** > **Message configuration**. In this case, we selected the following: **GGA**, **GSA**, **GSV**, **RMC**, **GST**. Feel free to select more depending on your application.

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
