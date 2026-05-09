# PROXmobil3 [In Progress]
Bus tappy card thing

# Instructions
## SSH
1. Plug in USB into computer
2. Open Disk utility (app)
3. Open External on left sidebar and click on the USB drive
4. Click Erase button on the top of the window
5. Format
    1. Name: anything
    2. Format: MS-DOS (FAT), not ExFat 
    3. Scheme: Master Boot Record
    4. Erase
6. Open Terminal
7. Create autorun.sh
    1. nano /Volumes/PROXUSB/autorun.sh
        1. note: since it is now a different format, it would be located under volumes. can confirm by looking at disk util
    2. [Script here](https://wiki.pm3.dev/ssh)
        1. replace key with actual public key
    3. Verify file is there
        1. ls -la /Volumes/PROXUSB/
    4. Eject
        1. Drag into Trash on Finder or diskutil eject /dev/disk2 
8. Plug into PM3
9. Turn on device
10. Let script run
11. “Find device’s IP address” ???
    1. ARP -a
12. SSH in: ssh root@IP

# Appendix
https://kevin.wallace.seattle.wa.us/pm3/
https://wiki.pm3.dev/start
https://wiki.pm3.dev/ssh
https://www.reddit.com/r/TriMet/comments/1qjaukx/want_your_own_hop_reader/
