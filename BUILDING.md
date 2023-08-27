# Building Anycubic Marlin source code

1. Obtain a Keil ARM Community license key via https://www.keil.arm.com/mdk-community/

1. Download and install Keil v5.36, do not install v5.37 as it doesn't ship with ARM Compiler v5.06 -> https://armkeil.blob.core.windows.net/eval/MDK536.EXE

2. Install the software as you would install any software and open it

3. The Pack Installer will open and start installing default packages (the progress bar is at the bottom right) . In the future if you want to open the Pack Installer it is located under Project -> Manage -> Pack Installer...

4. Once the default packages are installed, in the Pack tab on the right, find and install ARM::CMSIS 5.7.0 (2020-04-09) and uninstall the 5.8.0 version

5. Download and install HDSC.HC32F460 v1.0.7 -> https://github.com/ANYCUBIC-3D/HDSC_SupportPackage

6. Once the installation is done, close the Pack Installer and open Keil µVision 5

7. Go to File -> License Management...

8. Click on Get LIC via Internet... and click OK

9. On the next page, enter the license key you received for Keil

10. Enter a PC Description, a First Name, a Last Name, an E-mail, your country and your phone (everything else should be optional). The E-mail will be used to send you your activation code so make sure to input a real E-mail!

11. Press Submit on the bottom and wait to receive the E-mail

12. In the E-mail you will get a License ID Code (LIC), copy that code and go back to Licence Management in µVision

13. Paste the LIC in the New License ID Code (LIC) input and press Add LIC

14. Close the License Management tab and go to Project -> Open Project...

15. Open the anycubic.uvprojx file located in the workspace folder of the Anycubic source code (download it from Github)

16. You shouldn't have any error / message in the Build Output tab on the bottom, if it stays empty then it's good

17. To build, go to Project -> Build target

18. The output file will be located under workspace/firmware.bin
