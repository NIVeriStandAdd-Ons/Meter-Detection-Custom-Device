## Meter Detection Custom Device ##

**Meter Detection Custom Device** allows users to determine the position of a needle on a meter using an NI-IMAQdx compatible camera running within the NI VeriStand Engine.

### LabVIEW Version ###

LabVIEW 2012

### Built Availability ###

Builds are not available for this IP.

### Quality, Limitations ###

This IP was developed as a proof of concept (POC) for IMAQdx compatible cameras. Configuration for the custom device is done on the host side. Because of this, the user must have an available camera interface on both the host and target. As an example, when using a FireWire camera, the camera must be connected to the host during configuration. Prior to deployment the camera must be connected to the target. The camera on both the host and target must have the same camera interface name and settings. 

### Dependencies ###

NI-IMAQdx, NI Vision Development Module, 3rd party camera driver for certain cameras, NI-IMAQdx compatible camera

### Instructions for Use ###

1. Ensure the Camera Interface is set to the same name used in Measurement & Automation Explorer.
2. Set the external meter needle to the minimum possible value. Select Capture Image to capture an image of the needle.
3. Select the Line Tool on Image and draw a long along the length of the meter's needle. Select Set Min Meter ROI to set the minimum Region of Interest.
4. Set the external meter needle to the maximum possible value. Select Capture Image to capture an image of the needle.
5. Select the Line Tool on Image and draw a long along the length of the meter's needle. Select Set Max Meter ROI to set the maximum Region of Interest.
6. Ensure the Min Meter Value and Max Meter Value correspond to the minimum and maximum possible meter values respectively and set the Needle Configuration appropriately.
7. Save the system definition file.

### License ###

*This repository and any materials provided by NI therein are provided AS IS. NI DISCLAIMS ANY AND ALL LIABILITIES FOR AND MAKES NO WARRANTIES, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR  PARTICULAR PURPOSE, OR NON-INFRINGEMENT OF INTELLECTUAL PROPERTY. NI shall have no liability for any direct, indirect, incidental, punitive, special, or consequential damages for your use of the repository or any materials contained therein.*