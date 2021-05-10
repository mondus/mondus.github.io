# COM4521/COM6521 Lab Class Guidance

Lab classes for this module are held virtually with support available from instructors via the Mole (vle.sheffield.ac.uk) course rooms.

## Joining a lab class

1) Lab classes should be joined via Blackboard. Once you log in and select the module you will have alink on the main Module Content page for **Lab Class Session (Backboard Collaborate)**. This link will provide you with a list of lab sessions for each teaching week.

2) Once you have joined a session, to request help you can select the raise hand icon at the bottom of the screen. One of the lab demonstratiors will move you in to a private break-out room for discussion. 


## Logging into a machine

The majority of lab classes for this module require a computer with an NVIDIA GPU. The course [main page](../) has details of machines which are availabel to you. Connecting remotely to university machines requires:
* [2-factor authentication with mobile push notifications](https://sites.google.com/sheffield.ac.uk/mfa?pli=1&authuser=1).
* [Connecting to the university VPN](https://www.sheffield.ac.uk/it-services/vpn) (if you are not on the campus network).
* Mac users may need to install [Microsoft Remote Desktop](https://apps.apple.com/us/app/microsoft-remote-desktop/id1295203466?mt=12).

1) Connect to the university VPN. The legacy VPN system will be disabled during this semester, therefore it will be necessary to install the 'FortiClient' to use VPN. Guidenace for setting up the new VPN client on your local machine can be found [here](https://www.sheffield.ac.uk/it-services/vpn).

2) Visit [this page](https://www.sheffield.ac.uk/findapc/rdp/room/37/pcs) and select a free machine by clicking 'Connect' to download a remote desktop connection file.

![Connect to a pc](1.png "Connect to a pc")

3) Open the downloaded remote desktop connection file. You will be asked to enter you university password.

![Enter your password](2.png "Enter your password")

4) After entering your password, you should recieve a push notification from the Duo app on your mobile phone. If the notification has not appeared, try opening the app.  If this still fails, you likely don't have your account attached to that Duo app and may need to add it via the "Add a new device" option from the 2-factor authentication screen  when logging into the website.

![Push notification](3.jpg "Push notification")

5) When you first open Visual Studio 2019 on a remote machine you may be asked to login to validate the license.
Click "Check for an updated license", and select your user account.


![Visual Studio License](4.png "Visual Studio License")

6) You should now be ready to complete the lab classes. Materials for the lab classes can be downloaded from the [course website](https://paulrichmond.shef.ac.uk/teaching/COM4521/). This will be updated weekly to add the new lab material and the previous weeks lab solutions.

## Remote Assistance

You can share your Visual Studio session with a lab demonstrator by completing the following steps:

1)  In the top right corner of Visual Studio click the 'Live Share' button

![Live Share](7.png "Live share")

2) Click ok to pass the next dialog

![Firewall 1](8.png "Firewall 2")

3) Click cancel if a windows firewall dialog appears.

![Firewall 2](9.png "Firewall 2")

4) When live share has initialised, the "Live Share" button will change to "Sharing". Click it will now give you the option to copy the share link. Copy this link and send it to the lab assistant when you have been moved to a private room in the Mole classroom.

![Sharing](10.png "Sharing")

5) When the lab assistant has connected you should recieve a notification and they will appear as a participant in the Live Share panel.

![Participants](11.png "Participants")

6) Whilst providing support, the lab assistant may request access to edit/build/run your code. This will appear as a yellow bar. If the name of the request corresponds to a lab assistant, you should approve these requests.

![Request Access](12.png "Request Access")

7) It may also be necessary to share read/write access to a terminal window. (Remote participants cannot see the output window when debugging, but can execute the application manually from the shared terminal window).

![Request Access](13.png "Request Access")

**Note:** CUDA debugging is not currently supported during live sharing sessions, if the CUDA debugger break points into device code, the remote participant will be disconnected and unable to reconnect until the debugger has exited.

## CUDA Memory Checking

If using the next-gen CUDA debugger, it doesn't currently support CUDAMemcheck, so it will not report any memory access violations (for example if you are writing beyond the end of a buffer).

Therefore, it is necessary to use the standalone tool compute sanitizer.

This can be called from any command window using:

```
"C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.1\compute-sanitizer\compute-sanitizer.exe" --print-limit 1 <executable> (<run args>)
```

For example you might call:

```
"C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.1\compute-sanitizer\compute-sanitizer.exe" --print-limit 1 AdaptiveHistogramOptimisation.exe CUDA test_image.png
```

If a memory error is detected by any of your kernels, it will be reported similar to this:

```
========= COMPUTE-SANITIZER
========= Invalid __global__ write of size 4 bytes
=========     at 0x3c8 in U:/com4521/Lab04_Exercise01/exercise01_sln.cu:42:affine_decrypt_multiblock(int*,int*)
=========     by thread (0,0,0) in block (0,0,0)
=========     Address 0x4 is out of bounds
=========     Saved host backtrace up to driver entry point at kernel launch time
=========     Host Frame:GlobalInitializer [0x7ff8b9c080d4]
=========                in C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.1\compute-sanitizer\sanitizer-collection.dll
=========     Host Frame:GlobalInitializer [0x7ff8b9bc3fc7]
=========                in C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.1\compute-sanitizer\sanitizer-collection.dll
=========     Host Frame: [0x7ff8b9bac9b5]
=========                in C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.1\compute-sanitizer\sanitizer-collection.dll
=========     Host Frame: [0x7ff8b9bb39c8]
=========                in C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.1\compute-sanitizer\sanitizer-collection.dll
=========     Host Frame: [0x7ff8d6af79e0]
=========                in C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.1\compute-sanitizer\sanitizer-public.dll
=========     Host Frame:sanitizerUnsubscribe [0x7ff8d6afe1f1]
=========                in C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.1\compute-sanitizer\sanitizer-public.dll
=========     Host Frame: [0x7ff8b6fccde5]
=========                in C:\Windows\system32\DriverStore\FileRepository\nv_dispui.inf_amd64_bf0f2e72ecc4a6c6\nvcuda64.dll
=========     Host Frame:cuProfilerStop [0x7ff8b7162342]
=========                in C:\Windows\system32\DriverStore\FileRepository\nv_dispui.inf_amd64_bf0f2e72ecc4a6c6\nvcuda64.dll
=========     Host Frame: [0x7ff8b6e982fd]
=========                in C:\Windows\system32\DriverStore\FileRepository\nv_dispui.inf_amd64_bf0f2e72ecc4a6c6\nvcuda64.dll
=========     Host Frame: [0x7ff8b6e987ec]
=========                in C:\Windows\system32\DriverStore\FileRepository\nv_dispui.inf_amd64_bf0f2e72ecc4a6c6\nvcuda64.dll
=========     Host Frame: [0x7ff8b6e98ac4]
=========                in C:\Windows\system32\DriverStore\FileRepository\nv_dispui.inf_amd64_bf0f2e72ecc4a6c6\nvcuda64.dll
=========     Host Frame:cuLaunchKernel [0x7ff8b7060e14]
=========                in C:\Windows\system32\DriverStore\FileRepository\nv_dispui.inf_amd64_bf0f2e72ecc4a6c6\nvcuda64.dll
=========     Host Frame: [0x7ff8d6b8a5fa]
=========                in U:\com4521\x64\Debug\cudart64_110.dll
=========     Host Frame: [0x7ff8d6b8a4a6]
=========                in U:\com4521\x64\Debug\cudart64_110.dll
=========     Host Frame:cudaLaunchKernel [0x7ff8d6bad1c4]
=========                in U:\com4521\x64\Debug\cudart64_110.dll
=========     Host Frame:C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v11.1\include\cuda_runtime.h:211:cudaLaunchKernel<char> [0x7ff769fe221f]
=========                in U:\com4521\x64\Debug\Lab04_Exercise01.exe
=========     Host Frame:C:\Users\ac1rch\AppData\Local\Temp\tmpxft_000040a0_00000000-7_exercise01_sln.cudafe1.stub.c:9:__device_stub__Z25affine_decrypt_multiblockPiS_ [0x7ff769fe200d]
=========                in U:\com4521\x64\Debug\Lab04_Exercise01.exe
=========     Host Frame:C:\Users\ac1rch\AppData\Local\Temp\tmpxft_000040a0_00000000-7_exercise01_sln.cudafe1.stub.c:12:affine_decrypt_multiblock [0x7ff769fe1992]
=========                in U:\com4521\x64\Debug\Lab04_Exercise01.exe
=========     Host Frame:U:\com4521\Lab04_Exercise01\exercise01_sln.cu:78:main [0x7ff769fe1af0]
=========                in U:\com4521\x64\Debug\Lab04_Exercise01.exe
=========     Host Frame:D:\agent\_work\9\s\src\vctools\crt\vcstartup\src\startup\exe_common.inl:79:invoke_main [0x7ff769fe4879]
=========                in U:\com4521\x64\Debug\Lab04_Exercise01.exe
=========     Host Frame:D:\agent\_work\9\s\src\vctools\crt\vcstartup\src\startup\exe_common.inl:288:__scrt_common_main_seh [0x7ff769fe475e]
=========                in U:\com4521\x64\Debug\Lab04_Exercise01.exe
=========     Host Frame:D:\agent\_work\9\s\src\vctools\crt\vcstartup\src\startup\exe_common.inl:331:__scrt_common_main [0x7ff769fe461e]
=========                in U:\com4521\x64\Debug\Lab04_Exercise01.exe
=========     Host Frame:D:\agent\_work\9\s\src\vctools\crt\vcstartup\src\startup\exe_main.cpp:17:mainCRTStartup [0x7ff769fe4909]
=========                in U:\com4521\x64\Debug\Lab04_Exercise01.exe
=========     Host Frame:BaseThreadInitThunk [0x7ff901ec7c24]
=========                in C:\Windows\System32\KERNEL32.DLL
=========     Host Frame:RtlUserThreadStart [0x7ff902eed721]
=========                in C:\Windows\SYSTEM32\ntdll.dll
========= 
========= Target application returned an error
========= ERROR SUMMARY: 1026 errors
```

The first few lines have the most important information, the rest is a stack trace.

```
========= Invalid __global__ write of size 4 bytes
=========     at 0x3c8 in U:/com4521/Lab04_Exercise01/exercise01_sln.cu:42:affine_decrypt_multiblock(int*,int*)
=========     by thread (0,0,0) in block (0,0,0)
=========     Address 0x4 is out of bounds
```

Here we can see that there was an invalid write to global memory (as opposed to shared), by thread (0,0,0)(0,0,0) to the address 0x4.

This error was produced by writing the below code inside a cuda kernel, where it should be clear we are writing a 4 byte integer to the location 4 bytes past 0x0000 (nullptr).

```c
int *test = nullptr;
test[1] = 12;
```


