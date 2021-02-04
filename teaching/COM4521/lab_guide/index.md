# COM4521/COM6521 Lab Class Guidance

Lab classes for this module are held virtually with support available from instructors via the Mole (vle.sheffield.ac.uk) course rooms.

## Logging into a machine

The majority of lab classes for this module require a computer with an Nvidia GPU. You can access one of the suitable university machines remotley in [virtual class room 1](https://www.sheffield.ac.uk/findapc/rdp/room/37/pcs). Connecting remotely to university machines requires:
* [2-factor authentication with mobile push notifications](https://sites.google.com/sheffield.ac.uk/mfa?pli=1&authuser=1).
* [Connecting to the university VPN](https://www.sheffield.ac.uk/it-services/vpn) (if you are not on the campus network).
* Mac users may need to install [Microsoft Remote Desktop](https://apps.apple.com/us/app/microsoft-remote-desktop/id1295203466?mt=12).

1. Connect to the university VPN. The legacy VPN system will be disabled during this semester, therefore it will be necessary to install the 'FortiClient' to use VPN. Guidenace for setting up the new VPN client on your local machine can be found [here](https://www.sheffield.ac.uk/it-services/vpn).

2. Visit [this page](https://www.sheffield.ac.uk/findapc/rdp/room/37/pcs) and select a free machine by clicking 'Connect' to download a remote desktop connection file.

![Connect to a pc](1.png "Connect to a pc")

3. Open the downloaded remote desktop connection file. You will be asked to enter you university password.

![Enter your password](2.png "Enter your password")

4. After entering your password, you should recieve a push notification from the Duo app on your mobile phone. If the notification has not appeared, try opening the app.  If this still fails, you likely don't have your account attached to that Duo app and may need to add it via the "Add a new device" option from the 2-factor authentication screen  when logging into the website.

![Push notification](3.jpg "Push notification")

5. When you first open Visual Studio 2019 on a remote machine you may be asked to login to validate the license.
Click "Check for an updated license", and select your user account.


![Visual Studio License](4.png "Visual Studio License")

6. You should now be ready to complete the lab classes. Materials for the lab classes can be downloaded from the [course website](https://paulrichmond.shef.ac.uk/teaching/COM4521/). This will be updated weekly to add the new lab material and the previous weeks lab solutions.

## Recieving support during lab classes

1. *todo* How to connect to Mole meetings?

2. *todo* How to raise hand in Mole meetings?

3. In the top right corner of Visual Studio click the 'Live Share' button

![Live Share](7.png "Live share")

4. Click ok to pass the next dialog

![Firewall 1](8.png "Firewall 2")

5. Click cancel if a windows firewall dialog appears.

![Firewall 2](9.png "Firewall 2")

6. When live share has initialised, the "Live Share" button will change to "Sharing". Click it will now give you the option to copy the share link. Copy this link and send it to the lab assistant when you have been moved to a private room in the Mole classroom.

![Sharing](11.png "Sharing")

7. When the lab assistant has connected you should recieve a notification and they will appear as a participant in the Live Share panel.

![Participants](11.png "Participants")

8. Whilst providing support, the lab assistant may request access to edit/build/run your code. This will appear as a yellow bar. If the name of the request corresponds to a lab assistant, you should approve these requests.

![Request Access](12.png "Request Access")

9. It may also be necessary to share read/write access to a terminal window. (Remote participants cannot see the output window when debugging, but can execute the application manually from the shared terminal window).

![Request Access](13.png "Request Access")

**Note:** CUDA debugging is not currently supported during live sharing sessions, if the CUDA debugger break points into device code, the remote participant will be disconnected and unable to reconnect until the debugger has exited.


