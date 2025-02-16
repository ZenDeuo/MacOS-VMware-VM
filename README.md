# MacOS Ventura VMware Workstation Setup & Configuration!

## Guide:
## [Massive Thanks To](#back-to-the-top--massive-thanks-to)
## [System's Specifications That This Was Tested On](#back-to-the-top--systems-specifications-that-this-was-tested-on)
## [What To Expect Performance Wise From The VM](#back-to-the-top--what-to-expect-performance-wise-from-the-vm)
## [Prerequisites](#back-to-the-top--prerequisites)
## [Getting Started](#back-to-the-top--getting-started)
## [Creating The Virtual Machine](#back-to-the-top--creating-the-virtual-machine)
## [Prerequisites Before Configuring The Virtual Machine](#back-to-the-top--prerequisites-before-configuring-the-virtual-machine)
## [Configuring The Virtual Machine](#back-to-the-top--configuring-the-virtual-machine)
## [Installing MacOS (The Recovery Environment Setup Stage)](#back-to-the-top--installing-macos-the-recovery-environment-setup-stage)
## [Installing MacOS (The Out Of Box Experience Setup Stage)](#back-to-the-top--installing-macos-the-out-of-box-experience-setup-stage)
## [Installing VMware Tools](#back-to-the-top--installing-vmware-tools)
## [The End](#back-to-the-top--the-end)
## [Troubleshooting](#back-to-the-top--troubleshooting)

---

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | Massive Thanks To:
- [Tucano2000 For This Helpful Guide's Tools, All I've Really Done Is Added To It With Screenshots To Help The Users Better! Most Files You Find Here Will Be Further Updated Here Most Likely.](https://forum.amd-osx.com/threads/mac-os-install-on-amd-ryzen-vmware-opencore-improved-performance-works-with-sequoia-sonoma-etc.4696/)

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | System's Specifications That This Was Tested On: 
<li>OS: CachyOS (An Arch Based Distribution)</li><br>
<li>CPU: AMD Ryzen 9 7950X3D</li><br>
<li>GPU: AMD Radeon RX 7900 XTX</li><br>
<li>RAM: 64GB Corsair Vengeance</li><br>
<br>

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | What To Expect Performance Wise From The VM: 
The performance of the Virtual Machine is Usable for specific cases. You definitely couldn't game on it I know that much as the VMware Tools only gives you 128MB of Display Graphics to work with which is enough to do some simple Microsoft Office with and maybe just about use MacOS for testing before buying an actual Apple Mac. <br>
If you were looking to do Video Editing or Photoshop within this VM then I'm afraid this is where the fun ends pretty much as the Mac is already pretty unstable when Minimising & Maximising Windows, it lags severely so I highly doubt you'll be able to do much with Video Editing under such restricted conditions but I wish you luck Adventurer, You made it this far so maybe you can optimise the MacVM enough to run very well for your use cases!

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | Prerequisites: 
- Extraction Software Either: [7-Zip](https://7-zip.org/)  |  [WinRAR](https://www.win-rar.com/)  |  [PeaZip](https://peazip.github.io/)
- [Git](https://git-scm.com/downloads)
- VMware Workstation: [Link 1](https://blogs.vmware.com/workstation/2024/05/vmware-workstation-pro-now-available-free-for-personal-use.html)  |  [Link 2](https://support.broadcom.com/group/ecx/productdownloads?subfamily=VMware+Workstation+Pro)
- [VMware Unlocker](https://github.com/paolo-projects/auto-unlocker/releases)

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | Getting Started: 
This Guide should work on both Windows & Linux but no promises if it doesn't work because I've spent countless hours just trying to get it to work after people kept saying that it would never work and I was on the brink of giving up but if anything this just proves that even when your at the exit door and it's so easy to walk through, you should never give up!

So lets get started: <br>
Ensure that you have VMware Workstation installed. <br>
You can grab VMware Workstation from either of the following URL: <br>
[VMware's Website](https://blogs.vmware.com/workstation/2024/05/vmware-workstation-pro-now-available-free-for-personal-use.html) <br>
[Broadcom's Website](https://support.broadcom.com/group/ecx/productdownloads?subfamily=VMware+Workstation+Pro) <br>
<br>
Once you've finished downloaded and installing VMware Workstation, close VMware Workstation as you now need to Run and Install VMware Unlocker. <br>
To do this download [VMware Unlocker](https://github.com/paolo-projects/auto-unlocker/releases). (Press The Latest Version Of "Unlocker.zip" File to download it.) <br>
Extract it to the Downloads folder and follow the steps below: <br>
<li>For Windows Users</li><br>
Run Unlocker.exe and Install It / Follow What The GUI Interface Says, Then proceed to the Next Steps Below. <br>
<br>
<li>For Linux Users</li><br>
You'll need to compile the Code first before being able to execute it. <br>
I recommend reading their Guide under their "How To Use" and "Compile" Sections to get your VMware Workstation Unlocker working. Once you've Unlocked your VMware Workstation, Proceed to the Next Step Below.<br>
<br>

Open VMware Workstation and you should be met with an interface that looks a little something like this: <br>
![VMware Installer Image](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VMwareStartup.png)
<br>
<br>
Once you get to a page like this, you're going to want to clone this Repository. <br>
You may do so using the following command in either Command Prompt (CMD | Windows) or Terminal (Linux): <br>
<code>git clone https://github.com/ZenDeuo/MacOS-VMware-VM</code> <br>
<br>

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | Creating The Virtual Machine: 
Follow the Images below to correctly Setup your MacOS VM, I'll keep putting notes up here and there above some of the Images so ensure to keep an eye on those too whilst following the Installation Images. We'll talk more about configuring the Virtual Machine soon after you're done with this, Can't wait to see you at that stage! Oh and one more thing... (See what I did there) Just make sure your settings match what you see in the Images and press next, I haven't bothered editing these images for the moment but I will get round to editing them eventually so that it makes it clearer for those who are more Visual Learners rather than Text Learners :) <br>
<br>
To Start, Open VMware Workstation and in the Home Tab, Press "Create a New Virtual Machine" which will open this box: <br>
![VMware Workstation Setup Image 1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/1.png) <br>
<br>
![VMware Workstation Setup Image 2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/2.png) <br>
<br>
![VMware Workstation Setup Image 3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/3.png) <br>
<br>
![VMware Workstation Setup Image 4.0](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/4.0.png) <br>
<br>
![VMware Workstation Setup Image 4.1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/4.1.png) <br>
<br>
In the Image Below, Don't forget to give your MacOS VM a Custom Name so that the folder will match and you won't have to rename it after resulting in a VM and Folder Name Mismatch. It's just easier if you set a Name for it now; Also your location will look different to mine, I am running Linux whereas some of you if not the majority of people will be running Windows. Leaving this as the Default Location is completely okay, you **SHOULD NOT** have to modify this line after changing the VM Name. <br>
<br>
![VMware Workstation Setup Image 5](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/5.png) <br>
<br>
Below are 3 Images, If you click them; they'll open in a New Tab to make them easier to see. All that changes between them is the "Number of Cores per Processor". The options are 4, 8 and 16. You can choose how much Cores you give to your VM however your only options are 4, 8 and 16 so keep that in mind and input your chosen amount of cores into the VMware Workstation Software Create New Virtual Machine Window. <br>
This is required because you'll be extracting a Zip File soon containing the Boot VMDK File which allows you to boot OpenCore that allows MacOS to at least run in the VMware Workstation Software. <br>
<br>
<table align="center">
  <tr>
    <td width="33%"><a href="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/6.1-Minimum.png" target="_blank"><img src="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/6.1-Minimum.png" width="100%"/></a></td>
    <td width="33%"><a href="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/6.2-Middle-Recommended.png" target="_blank"><img src="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/6.2-Middle-Recommended.png" width="100%"/></a></td>
    <td width="33%"><a href="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/6.3-Maximum.png" target="_blank"><img src="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/6.3-Maximum.png" width="100%"/></a></td>
  </tr>
</table>
<br>
Below are 4 Images; You may press the Images to open them in a New Tab to better view them. These Images are for the VM's RAM Configuration. 4GB's of RAM being the Lowest you should give the MacVM, 8GB's of RAM being the Recommended Amount to give the MacVM, 16GB's of RAM being a High Amount of RAM to give the VM and then finally 32GB's+ being Overkill and well more than enough however only you know how much RAM you need, not me! <br>
<br>
<table align="center">
  <tr>
    <td width="25%"><a href="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/7.1-Minimum.png" target="_blank"><img src="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/7.1-Minimum.png" width="100%"/></a></td>
    <td width="25%"><a href="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/7.2-Middle-Recommended.png" target="_blank"><img src="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/7.2-Middle-Recommended.png" width="100%"/></a></td>
    <td width="25%"><a href="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/7.3-Maximum.png" target="_blank"><img src="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/7.3-Maximum.png" width="100%"/></a></td>
    <td width="25%"><a href="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/7.4-Overkill-UpToYou.png" target="_blank"><img src="https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/7.4-Overkill-UpToYou.png" width="100%"/></a></td>
  </tr>
</table>
<br>

![VMware Workstation Setup Image 8](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/8.png) <br>
<br>
![VMware Workstation Setup Image 9](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/9.png) <br>
<br>
![VMware Workstation Setup Image 10](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/10.png) <br>
<br>
![VMware Workstation Setup Image 11](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/11.png) <br>
<br>
For the Image Below; Ensure that you set this Virtual Disk to "Store virtual disk as a single file" so that you can easily move it between Systems, It also is more performant this way too (Or so I've heard; Can't confirm it, however it's better off if you choose the Store Option as this is how I did it.). <br>
<br>
![VMware Workstation Setup Image 12](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/12.png) <br>
<br>
![VMware Workstation Setup Image 13](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/13.png) <br>
<br>
On the Image below you can just press Finish but **DO NOT** Boot the Machine in its Current State as it will not Boot. <br>
There is still a little more Configuration to get through first but after the new Configurations are done **THEN** you can Boot the VM and have some fun! <br>
<br>
![VMware Workstation Setup Image 14](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Setup/14.png) <br>
<br>

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | Prerequisites Before Configuring The Virtual Machine:
Remember during Setup choosing "Number of Cores per Processor"? If not, you can quickly figure it out by going to: <br>
Your VM --> Edit Virtual Machine Settings --> Processors <br>
Now that you know the Number of Cores you selected during Setup, you'll need to go to the folder where you Cloned this Repository to and head into the "MacOS OpenCore Patchers" Folder. <br>
In this folder you'll see 3 Zip Files: <br>
<li>MacOS OpenCore V1.0 VM 4 Cores Version.zip</li><br>
<li>MacOS OpenCore V1.0.1 VM 8 Cores Version.zip</li><br>
<li>MacOS OpenCore V1.0.1 VM 16 Cores Version.zip</li><br>
You must choose the Version that has the same amount of Cores that corresponds to the amount of Cores you put into the VM. So if in the VM you selected 8 Cores per Processor, you'll be using the VM 8 Cores Version. <br>
Go ahead and Extract the File inside of your chosen ZIP and leave it in a memorable place or put it in your VM Folder often located in these places: <br>
Windows: C:\Users\USERNAME\Documents\Virtual Machines <br>
Linux: /home/USERNAME/vmware <br>
<br>
Once you've stored it in a memorable place you need to keep this file for the VM to Boot, so keep that in mind! <br>
You may now move on to Configuring The Virtual Machine! <br>
<br>
PS. If this is the first time you are doing this Step, please ignore the Jump Back To Configuring The VM and proceed with the Images Below. <br>
However if you came back here because you happened to have forgotten where you put the extracted file and have re-extracted the file or found the file you extracted and then lost, You may jump back to the Configuring VM Point you were at below: <br>

#### [Jump Back To Configuring The VM](#if-you-forgot-youll-be-jumped-back-here-and-can-continue-reading-forth)
<br>

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | Configuring The Virtual Machine:
Time to Configure your Virtual Machine! After this is done, You can then Install and Boot MacOS. YIPPIE! <br>
<br>
![VMware Workstation Configuration Image 1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/1.png) <br>
<br>
![VMware Workstation Configuration Image 2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/2.png) <br>
<br>
![VMware Workstation Configuration Image 3.1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/3.1.png) <br>
<br>
![VMware Workstation Configuration Image 3.2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/3.2.png) <br>
<br>
![VMware Workstation Configuration Image 3.3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/3.3.png) <br>
<br>
![VMware Workstation Configuration Image 4.1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/4.1.png) <br>
<br>
![VMware Workstation Configuration Image 4.2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/4.2.png) <br>
<br>
![VMware Workstation Configuration Image 4.3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/4.3.png) <br>
<br>
![VMware Workstation Configuration Image 4.4](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/4.4.png) <br>
<br>
![VMware Workstation Configuration Image 4.5](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/4.5.png) <br>
<br>
Remember that file you Extracted and put in a Memorable Location? You performed this task as part of the [Prerequisites Before Configuring The Virtual Machine.](#back-to-the-top--prerequisites-before-configuring-the-virtual-machine) <br>
If you forgot that's okay just go ahead and redo the tasks in Prerequisites Before Configuring The Virtual Machine and then come back here. <br>
I've included a Jump Button in that Section too in case you struggle to find this place again! :) <br>
<br>
### If You Forgot You'll Be Jumped Back Here And Can Continue Reading Forth!
Anyways that file will be used here in the Image Above! <br>
Below is the Visual Representation of what mine looks like so that you know you're selecting the right file too as they'll all look similar! <br>
Now that you know, You can venture forth! <br>
<br>
![VMware Workstation Configuration Image 4.6](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/4.6.png) <br>
<br>
![VMware Workstation Configuration Image 4.7](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/4.7.png) <br>
<br>
![VMware Workstation Configuration Image 4.8](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/4.8.png) <br>
<br>
![VMware Workstation Configuration Image 5.1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/5.1.png) <br>
<br>
![VMware Workstation Configuration Image 5.2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/5.2.png) <br>
<br>
![VMware Workstation Configuration Image 5.3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/5.3.png) <br>
<br>
![VMware Workstation Configuration Image 5.4](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/5.4.png) <br>
<br>
![VMware Workstation Configuration Image 5.5](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/5.5.png) <br>
<br>
![VMware Workstation Configuration Image 5.6](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/5.6.png) <br>
<br>
Now you'll need to Select Your ISO File for MacOS Ventura, You can easily create one if you have a spare Mac or you could download one from the [Internet Archive](https://archive.org)... For Example: [Internet Archive: MacOS Ventura 13.0](https://archive.org/details/mac-os-ventura-13.0/macOS%2013-2022-12-22-22-18-37.png) or [Internet Archive: MacOS Ventura And Sonoma](https://archive.org/details/macos-ventura-and-sonoma). I don't think I can legally provide ISO Files however those link to ISO files uploaded by other users that should work just as well as my Ventura ISO... <br>
The way I got my ISO was from [these lovely people here](https://github.com/kholia/OSX-KVM/) who have created something similar but instead for QEMU which allows for GPU Passthru so it only works ideally if you've got 2 GPU's and 1 of them is supported via the Mac Operating System. <br>
You may use their file: [fetch-macOS-v2.py](https://github.com/kholia/OSX-KVM/blob/master/fetch-macOS-v2.py) Python File which I've also uploaded here just in case theirs disappears but hopefully it won't as theirs will always be the most up-to-date one so please use theirs if possible as my reupload won't be maintained regularly! <br>
<br>
Once you've got an ISO and put it in the VM, you can continue with the Installation! <br>
<br>
![VMware Workstation Configuration Image 5.7](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/5.7.png) <br>
<br>
![VMware Workstation Configuration Image 5.8](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/5.8.png) <br>
<br>
![VMware Workstation Configuration Image 5.9](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/5.9.png) <br>
<br>
![VMware Workstation Configuration Image 6.1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/6.1.png) <br>
<br>
![VMware Workstation Configuration Image 6.2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/6.2.png) <br>
<br>
![VMware Workstation Configuration Image 6.3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/6.3.png) <br>
<br>
Right, now you get to do the most Exciting THING and WATCH IT COME TO LIFE! Press the "Start up this guest operating system" as the button says and wait for it to Post and Boot into the OpenCore Bootloader then proceed with the [Installing MacOS Guide!](#back-to-the-topmacos-ventura-vmware-workstation-setup--configuration--installing-macos) <br>
<br>
![VMware Workstation Configuration Image 7](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/VM-Configuration/7.png) <br>
<br>


### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | Installing MacOS (The Recovery Environment Setup Stage): 
So let's begin with Setting Up MacOS in the VM! <br>
Start the Virtual Machine if you already haven't and follow the Pictures below for Visual Setup Instructions! <br>
As always, I'll be adding notes above Images I think are worthy to have notes added above and also to assist you more if you are to encounter the same or similar issues to me you can follow the note steps and continue with your MacOS Installation. <br>
I should note, I've **ONLY** tested this with MacOS Ventura so I can't promise it'll work with Newer or Older Versions of MacOS. You have been warned. <br>
Good luck with the Setup and HAVE FUN! <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/1.png) <br>
<br>
If your System runs into this Error or Kernel Panic, You can tell it's had a panic because it says at the bottom <code>"end nested panic string."</code> <br>
To fix this issue (For me at least it fixed the issue), I figured that Stopping the Virtual Machine, Closing VMware Workstation and then Relaunching VMware Workstation and Starting the VM back up fixed it for me, but you may have to reboot your Machine if you're on Windows as VMware doesn't entirely close unless you kill it entirely through Task Manager, but I recommend a System Reboot if restarting VMware Workstation doesn't fix the issue. <br>
After the issue is fixed, Just continue to Image 3 as you would! <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/2.png) <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/3.png) <br>
<br>
(Image Below) It's Booting!... (Most Likely). When it's doing this cool text stuff, just as long as it keeps moving its working (I Hope). <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 4](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/4.png) <br>
<br>
(Image Below) Select your language and continue to the image below! <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 5](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/5.png) <br>
<br>
(Image Below) Now we have to setup the Virtual Disk we configured during the VM Setup Stage. To do this; press on "Disk Utility" and then press "Continue" and continue to the Next Image for more information! <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 6.1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/6.1.png) <br>
<br>
(Image Below) Select the Drive that should be named "VMware Virtual SATA Hard Drive Media", Make sure it has around the same amount you configured it to have during the VM's Creation, if it looks like it's in use or is the incorrect size then it most likely the wrong drive. If the drive doesn't appear then you may have incorrectly set up the Virtual Disk, In this case, proceed to [Troubleshooting](#back-to-the-topmacos-ventura-vmware-workstation-setup--configuration--troubleshooting) by pressing the word Troubleshooting or by scrolling to the bottom of the page, once you've fixed your issue; come back here and continue setup. <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 6.2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/6.2.png) <br>
<br>
(Image Below) Press Erase in the top portion of the Disk Utility Application. <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 6.3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/6.3.png) <br>
<br>
(Image Below) Name the Drive whatever you like, keep in mind however that this drive cannot be renamed once it's name is set, it's set in stone as far as I'm aware. Then press the Blue "Erase" Button and proceed to the next image! <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 6.4](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/6.4.png) <br>
<br>
(Image Below) It'll begin formatting as it should. <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 6.5](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/6.5.png) <br>
<br>
(Image Below) Once it's done formatting, press the Blue "Done" Button. <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 6.6](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/6.6.png) <br>
<br>
(Image Below) Now in the top left, press "Disk Utility" then in the Dropdown that appears, Press "Quit Disk Utility" and you'll be returned to the menu you were at before you opened Disk Utility. <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 6.7](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/6.7.png) <br>
<br>
(Image Below) Press "Install macOS Ventura" and then press the Grey "Continue" Button. <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 7](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/7.png) <br>
<br>
(Image Below) Press the Blue "Continue" Button on this screen. <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 8.1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/8.1.png) <br>
<br>
(Image Below) "Agree" To the Terms of the Software License Agreement. <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 8.2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/8.2.png) <br>
<br>
(Image Below) Press Agree again... <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 8.3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/8.3.png) <br>
<br>
(Image Below) Select the drive you just formatted within Disk Utility and press the Grey "Continue" Button to proceed forth. <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 8.4](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/8.4.png) <br>
<br>
(Image Below) Now just wait for it to install! <br>
Note: It will reboot a lot so just leave it be and let it boot as it should, if you accidentally nudge the mouse or the keyboard during reboots on the OpenCore Bootloader then just make sure you select the "macOS Installer" option to proceed with the installation as normal :) <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 8.5](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/8.5.png) <br>
<br>
(Image Below) Accidentally nudge the mouse or the keyboard during reboots on the OpenCore Bootloader? It's okay, Just make sure you select the "macOS Installer" option to proceed with the installation as normal :) <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 9.1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/9.1.png) <br>
<br>
(Image Below) Just keep waiting, I promise it'll be worth it if this is what you want at least! <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 9.2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/9.2.png) <br>
<br>
(Image Below) If you happen to get stuck on this screen but it says "Shutting Down" then you may safely assume as long as the text doesn't move for longer than 20 seconds that the VM has shutdown but is stuck, so you can go ahead and press the Reboot button at the top of VMware Workstation Software, It should look like 2 Arrows going round in a circular motion if that helps :) <br>
Once you've rebooted just proceed with the installation as normal! <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 9.3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/9.3.png) <br>
<br>
(Image Below) If you see that the Boot Device has been renamed to what you named it in Disk Utility then that means you're almost finished with the installation! <br>
Just a few more minutes to go! Remain calm and grab yourself a coffee or 2 and let it do its thing! <br>
<br>
![Apple MacOS Ventura Recovery Environment Setup Instruction Image 9.4](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/Recovery-Environment-Setup/9.4.png) <br>
<br>

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | Installing MacOS (The Out Of Box Experience Setup Stage):
Now that you've completed the MacOS Recovery Environment Setup Steps, you can now finally follow these steps, get VMware Tools setup and you're good to go! <br>
Just keep in there! We're nearly done! <br>
<br>

![Apple MacOS Ventura OOBE Setup Instruction Image 1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/1.png) <br>
<br>
Welcome to MacOS Ventura! Set it up as you would and then once you're at the Desktop we can get to installing the Final Boss, VMware Tools :o ... See you there! <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/2.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/3.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 4](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/4.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 5](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/5.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 6](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/6.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 7](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/7.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 8](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/8.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 9](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/9.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 10](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/10.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 11](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/11.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 12](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/12.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 13](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/13.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 14](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/14.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 15](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/15.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 16](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/16.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 17](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/17.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 18](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/18.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 19](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/19.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 20](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/20.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 21](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/21.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 22](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/22.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 23](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/23.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 24](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/24.png) <br>
<br>
(Image Below) For the Migration Assistant, I wouldn't recommend using it, however if you would like to, then you may go ahead and do so, Just make sure you don't sign in to iCloud as this Machine has not been configured with Fake Information meaning Apple may lock your account and/or subsequently ban your account permanently so please be careful! <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 25](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/25.png) <br>
<br>
(Image Below) **DO NOT SIGN IN, DO NOT SIGN IN, DO NOT SIGN IN**. As stated in the last note; This VM has not been configured with Fake Information meaning Apple may lock your Account and/or subsequently ban your account permanently for using a Fake System that isn't brought from Apple directly because they can't verify that your Machine, in this case the VM, is Genuine or not. So please do not sign in. <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 26](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/26.png) <br>
<br>
(Image Below) Continue to Skip. <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 27](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/27.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 28](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/28.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 29](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/29.png) <br>
<br>
(Image Below) Create your account how you want it! <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 30](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/30.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 31](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/31.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 32](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/32.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 33](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/33.png) <br>
<br>
(Image Below) Wouldn't Recommend Enabling Location Features but it's up to you, not that it does anything really since most computers don't have any GPS or anything. <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 34](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/34.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 35](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/35.png) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 36](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/36.png) <br>
<br>
(Image Below) Ensure you disable this (Share Mac Analytics with Apple), as it's a Fake Mac they could start eyeing the information being sent to their servers and do something to your Machine if they can, I'm not too sure, Personally however I would highly recommend disabling this option. <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 37](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/37.png) <br>
<br>
(Image Below) Yep, Just like that; and proceed :) <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 38](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/38.png) <br>
<br>
(Image Below) You don't have to set this up but I much prefer it so I went ahead and chose to continue with it, However as I said you don't have to! <br>
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 39](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/39.png) <br>
<br>
(Image Below) Welcome to your MacOS Desktop! YOU MADE IT! I am very proud of you and this guide since it took so long to write and it's very exhausting both writing, checking it over consistently, making sure what I'm writing down works on my Machine etc. <br>
However, Congratulations User! You did it and now this last step should be very easy to perform (I hope) <br>
Just follow the steps below in [Installing VMware Tools](#back-to-the-topmacos-ventura-vmware-workstation-setup--configuration--installing-vmware-tools) and you'll be well on your way to a functioning well enough VM for your needs hopefully.
<br>
![Apple MacOS Ventura OOBE Setup Instruction Image 40](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-Setup/OOBE-Setup/40.png) <br>
<br>

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | Installing VMware Tools: 
Now follow the steps below; and you'll be well on your way to a functioning well enough VM for your needs... Hopefully.
<br>
(Image Below) Open Safari... <br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 1](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/1.png) <br>
<br>
(Image Below) Naviage to Broadcom's Support Page: <code>https://support.broadcom.com/</code> <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 2](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/2.png) <br>
<br>
(Image Below) If you don't have a Broadcom Account then you'll need to Register for one, Broadcom brought VMware so everything goes through them now. <br>
If you're having issues getting to specific pages on Broadcom's Site using Safari look at the text above the Next Image for a Solution. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 3](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/3.png) <br>
<br>
(Image Below) If you're having an issue getting to the Login Page where it tries to open the Tab in a New Tab but doesn't open the tab, Right Click the Login or Register Button and open it in a New Tab. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 4](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/4.png) <br>
<br>
(Image Below) Sign up as you would or if you already have an account, Open the Login Page and continue logging into your account. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 5](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/5.png) <br>
<br>
(Image Below) Once you're logged in, You want to make your way to the next URL being: <code>https://support.broadcom.com/group/ecx/productfiles?subFamily=VMware%20Tools&displayGroup=VMware%20Tools%2012.x&release=12.3.5&os=&servicePk=203561&language=EN</code> <br>
<br>
View The Next Image's Notes <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 6](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/6.png) <br>
<br>
(Image Below) Where my Mouse Pointer goes big, there may be a Checkbox there for you to Accept the Terms & Conditions before downloading?? Weird Placement, took me forever to notice the box even existed and it annoyed me once I found it because it's such a stupid place to put such a pointless button in my Opinion. <br>
Once you've checked that Box it should let you download the MacOS VMware Tools Zip File (I hope). <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 7](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/7.png) <br>
<br>
(Image Below) Yep just download this one. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 8](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/8.png) <br>
<br>
(Image Below) To download the File, Press this download button. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 9](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/9.png) <br>
<br>
(Image Below) Now Press the Blue Allow Button to let Safari download the Zip File. <br>
Safari may also Auto-Extract the Zip file for you too meaning you'll be able to just instantly jump into the Folder and start the Installation, If it didn't just double click the Zip File in Finder --> Downloads and it should begin Auto-Extracting! <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 10](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/10.png) <br>
<br>
(Image Below) Open The Folder. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 11](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/11.png) <br>
<br>
(Image Below) Open The Darwin.iso. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 12](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/12.png) <br>
<br>
(Image Below) Run "Install VMware Tools". <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 13](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/13.png) <br>
<br>
(Image Below) Press "Open". <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 14](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/14.png) <br>
<br>
(Image Below) Press "Continue". <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 15](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/15.png) <br>
<br>
(Image Below) Press "Install". <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 16](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/16.png) <br>
<br>
(Image Below) Provide it with your MacOS Account Password that you Setup in the Out Of Box Experience and leave it to run through. <br>
If any popup boxes appear, Do your best to press "OK", "Accept" etc on the boxes. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 17](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/17.png) <br>
<br>
(Image Below) Once you get to this stage, On one of the boxes press "Open System Settings". <br>
Move to the Next Image's Notes Below. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 18](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/18.png) <br>
<br>
(Image Below) Press "Allow". <br>
Next Image's Notes Below. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 19](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/19.png) <br>
<br>
(Image Below) **ENSURE YOU PRESS NOT NOW, ENSURE YOU PRESS NOT NOW, ENSURE YOU PRESS NOT NOW**. <br>
Next Image's Notes Below. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 20](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/20.png) <br>
<br>
(Image Below) It should say "The installation failed." in the Install VMware Tools window, If so that's correct behaviour, because MacOS was blocking VMware from installing its Kernel Modules, You've now allowed it through the settings. <br>
You should press "Close" on that box and go to the Next Image's Notes. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 21](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/21.png) <br>
<br>
(Image Below) Reopen "Install VMware Tools and continue the Installation as you did when you first ran the Program. <br>
Proceed to the Next Image's Notes. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 22](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/22.png) <br>
<br>
(Image Below) The installation should succeed as it shows below, If not and you got more popups, be sure to "Allow", "Agree", "OK", "Yes", "Open System Settings" etc on those Boxes and do as it tells you, if you need to allow VMware Kernel Modules again, do so then rerun this installer. <br>
Now press "Restart" and your MacVM should reboot. If it doesn't when it freezes just press the Reload Icon in VMware Workstation's Software and it should restart the MacOS System. <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 23](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/23.png) <br>
<br>
(Image Below) Once you've Rebooted and Logged in, you should already see the change, the Resolution should be 1920x1080 and if you open the following below: <br>
Next Image's Notes... <br>
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 24](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/24.png) <br>
<br>
(Image Below) You should see "Graphics Display 128 MB" as it should be, this means VMware Tools installed correctly and with no issue. <br>
If your MacOS VM does not reflect these changes listed in the Notes like the Resolution Change and the "Graphics Display 128 MB" Change shown in About This Mac, then you may need to reinstall the VMware Tools again from the same place and reboot and then they should be fully functioning!
<br>
![Apple MacOS Ventura VMware Tools Installation Instruction Image 25](https://cdn.deuo.one/Files/PICS/VMware-Workstation-MacOS-Ventura/Apple-Ventura-VMware-Tools-Setup/25.png) <br>
<br>

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | The End: 
<br>
AND CONGRATULATIONS USER, YOU HAVE MADE IT TO THE END!
I AM VERY PROUD THAT THIS GUIDE HELPED YOU INSTALL MACOS VENTURA IN VMWARE!
I hope you can share this around to your friends that want to run MacOS and whoever else just want to use MacOS for some of the things they might want to do in MacOS that maybe they can't do in any other OS.
Or maybe they just prefer to use MacOS for Microsoft's Office Suite for example, Whatever the reason, I'm sure this VM should be able to hand some of the tasks you throw at it as long as it's not too heavy like Blender or Photoshop / Video Editing.

### ([Back To The Top](#macos-ventura-vmware-workstation-setup--configuration)) | Troubleshooting: 
Welcome to the Troubleshooting Section! <br>
This should give you some Common Fixes for issues you may be encountering! <br>
<br>
<li>Virtual Disk Doesn't Show Up In MacOS Installer</li> <br>
To fix this issue, Shutdown your MacOS Installation --> Edit virtual machine settings: <br>
Ensure you have 2 Hard Disk's, Should be named something like: Hard Disk (SATA) and Hard Disk 2 (SATA). <br>
If you do not have 2 Hard Disk's then you need to create the Main OS Hard Disk. You can do this by following the steps below: <br>
<li>Press Add...</li>
<li>Hard Disk.</li>
<li>SATA (Recommended).</li>
<li>Create a New Virtual Disk.</li>
<li>Input the Size you want for the Virtual Disk and select "Store Virtual Disk as a Single File".</li>
<li>Press Next.</li>
<li>Press Finish.</li>
<br>
On the new Selected Drive, should be named something like "New Hard Disk (SATA)", Select it in the Left Menu: <br>
<li>Press "Advanced"</li>
<li>Change the Virtual Device Node to SATA 0:2 (If it isn't already on SATA 0:2</li>
<li>Press Close</li>
<li>Press Save</li>
<li>Try Installing MacOS Again.</li>
<br>
If you have the Drive, ensure it says "Hard Disk (SATA)" if it doesn't, this likely means you chose a different option during setup meaning you're going to have to Remove that Virtual Disk by Selecting it in the Left Menu and then pressing Remove at the Bottom in "Edit virtual machine options" then follow the text guide a few lines above this. <br>
<br>

### Issues Picked Up In Tucano2000's Guide.

### White Background / Wallpaper In MacOS: 
If when you first get into MacOS you have the problem where the Background / Wallpaper is White. <br>
<li>Navigate into System Settings</li>
<li>Wallpaper Settings</li>
<li>Deactivate the "Show as Screen Saver" Option</li>
<li>Then choose a wallpaper you like :)</li>
<br>

### SLOW UPLOAD SPEED: 
If there's a problem with your File Upload over the Network / Internet, You can fix this by: <br>
<br>
Open the Mac Terminal and type the Commands below in order: <br>
<br>
<li><code>sudo sysctl -a | grep net.inet.tcp.tso</code></li> <br>
<li><code>sudo sysctl -w net.inet.tcp.tso=0</code></li> <br>
<li><code>sudo nano /etc/sysctl.conf</code></li> <br>
<br>
Add the below entry in the sysctl.conf File: <br>
<li><code>net.inet.tcp.tso=0</code></li> <br>
<br>
Press Control + O then Enter to Save then press Control + X to exit.Restart your MacOS VM.
<br>
This happens due to a problem with the VMware vmxnet3 Network Driver.
<br>
Tucano2000 has tested this solution and managed to solve this problem with the steps above.
<br>

### For Windows Only: 
This should help improve the performance of the Virtual Machine and correct some Errors during Startup. <br>
<br>
Turning Off The Windows Hypervisor: <br>
<li>In Windows, Open the Start Menu and Search for "Command Prompt"</li>
<li>Right-Click "Command Prompt" and then click "Run as Administrator".</li>
<li>If the User Account Control dialog box appears, Confirm that the Action shown is the one you want to proceed with and click Continue.</li>
<li>Then type: “<code>bcdedit /set hypervisorlaunchtype off</code>” Hit Enter.</li>
<li>Then type: <code>reg add “HKLM\SYSTEM\CurrentControlSet\Control\DeviceGuard\Scenarios\HypervisorEnforcedCodeIntegrity” /v “Enabled” /t REG_DWORD /d 0 /f</code></li>
<li>Press enter again.</li>
<li>Restart your Computer (Not the VM).</li>
<br>
- It is also recommended to disable the "Memory Integrity Checks" in Windows to Improve the Performance. <br>
After installing VMware Tools, you may only change the Resolution within MacOS. Ex: 1600x1100. To do this, <br>
<br>
- Type in the MacOS Terminal: <code>sudo /Library/Application\ Support/VMware\ Tools/vmware-resolutionSet 1600 1100</code> <br>
Note: In VMWare's Display Settings you need to set the Resolutions Higher than or Equal to the ones you'll be using in macOS. <br>
THIS WAY YOU CAN EVEN RUN XCODE SIMULATOR SMOOTHLY AT LOW RESOLUTIONS SUCH AS 1024X768.
