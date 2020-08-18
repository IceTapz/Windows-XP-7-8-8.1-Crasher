# Windows-XP-7-8-8.1-Crasher
A Windows XP/7/8/8.1 Crasher with a single line of JavaScript.

# Description
This exploits a vulnerability in Windows XP to Windows 8.1. The master file table, or MFT, is a hidden file in the NTFS file system. It maps out all files in the drive. It is supposed to be protected from any user access because all files that use NTFS have a reference to it. If the directory is recreated, the system will lock the file until the next reboot. Therefore, for example, when trying to create a file or read the volume of files, NTFS attempts to seize ERESOURCE $ MFT file and will hang at this stage forever.

# Exploit
The exploit tries to access a nonexistant file c:/$MFT/pwned. The browser will hang then stop responding, then after the browser exits, the rest of the system becomes unresponsive.

**Tested on:** Windows XP/7/8/8.1

**Exploit Author:** EagleWire

**Date:** 6\23\17

**CVE:** N/A
**CVSS:** N/A
**ExploitDB ID:** 42253

# Protection
Couldn't find anything about this, however this doesn't affect Windows 10 so what are you waiting for if you haven't updated already?
