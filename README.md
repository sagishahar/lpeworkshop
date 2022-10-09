# Windows / Linux Local Privilege Escalation Workshop

My give back to the community initiative that was presented for free at several private and public events across Australia:

* Sydney - PlatypusCon (2017)
* Perth - BsidesPerth (2017)
* Brisbane - CrikeyCon (2018)

The workshop is based on the attack tree below, which covers all known (at the time) attack vectors of local user privilege escalation on both Linux and Windows operating systems.
<img src="https://pbs.twimg.com/media/DAZsE2VUQAA_bpZ.jpg">

### Material

* [Workshop Slide Deck](https://github.com/sagishahar/lpeworkshop/blob/master/Local%20Privilege%20Escalation%20Workshop%20-%20Slides.pdf)
* Exercise Worksheets ([Linux](https://github.com/sagishahar/lpeworkshop/blob/master/Lab%20Exercises%20Walkthrough%20-%20Linux.pdf), [Windows](https://github.com/sagishahar/lpeworkshop/blob/master/Lab%20Exercises%20Walkthrough%20-%20Windows.pdf))
* [Lab VM for Linux Exercises](https://www.icloud.com/iclouddrive/0c5M0j7milKwffvV_FcrO0oZg#Debian_6_64-bit_(Workshop)) (username: user / password: password321, username: root / password: password123)
* [Kali VM for Linux/Windows Exercises](https://www.icloud.com/iclouddrive/00ehXImzPdj4hJ3W-lC2PVOKQ#Kali_2016.2_x64_(Workshop)-003) (root:toor)
* [Videos for Windows Exercises](https://www.youtube.com/playlist?list=PLjG9EfEtwbvIrGFTx4XctK8IxkUJkAEqP)
* [Tools for Windows Exercises](https://www.icloud.com/iclouddrive/081l40jNtagOQNaHCACMN5_sQ#tools) (7z archive password: lpeworkshop)
* [Windows exercises setup script](https://github.com/sagishahar/lpeworkshop/blob/master/lpe_windows_setup.bat)

### Setup Instructions for Windows
1. Start a Windows VM that you legitimately own
2. Login to the Windows VM using a user account that has administrator privileges
3. Ensure the Windows VM does not have a user account named 'user'. If it exists, delete it
4. Copy the setup script (lpe_windows_setup.bat) to a writeable location on a Windows VM (the Desktop directory is fine)
5. Right click on the copied setup file and ensure to select from the pop-up menu 'run as Administrator'
6. Read carefully the output of the script
7. Restart the Windows VM
8. Copy the Tools 7z archive to the Desktop and extract it
9. Setup is now complete, enjoy

The script was developed and tested on a Windows 7 (SP1) x64 Build 7601 English-US host. It might work on other OS instances, but it is not guaranteed. Pay attention to the script's output. Some exercises are skipped (e.g. Kernel, etc.) as it depends on the patchlevel of the VM.

NOTE: As with any intentionally vulnerable hosts, ensure the Windows VM is not connected to an externally facing network.

