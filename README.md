# P0VsRedHerring
"Luckily, there are underground 0day exploits for FTPD for path traversal." #FakeNews #DotDotWontPwn #JailBreak #DJI #Spark

Update: This vulnerability has been addressed in DJI Spark Aircraft Firmware: V 01.00.0500 
https://forum.dji.com/thread-106245-1-1.html

Update: This vulnerability has been addressed in DJI Mavic Aircraft Firmware: V 01.03.1000


/system is now "ro" instead of "rw", and tar no longer follows hard or soft links, effectively neutering the original variant.

Lets examine POV's claims and red herrings. I've been chasing them for over a month or so... They make complete sense now. 
https://www.rcgroups.com/forums/showpost.php?p=36232471&postcount=15113
```
"BusyBox FTPD is running on all interfaces, but unlike Phantom 3, in Mavic it's restricted to '/ftp' directory." 
"Luckily, there are underground 0day exploits for FTPD for path traversal." 
"I can confirm that you can traverse out of the '/ftp' directory and reach the init scripts to set debug flag.  
```

![Murica](http://weknowmemes.com/wp-content/uploads/2014/07/4th-of-july-memes.jpg)

[![Fuck yeah](https://github.com/MAVProxyUser/P0VsRedHerring/raw/master/Still.jpeg)](https://www.youtube.com/watch?v=BTQ_CTih1HM)

![thx P0V](https://github.com/MAVProxyUser/P0VsRedHerring/raw/master/BigUps.jpg)

### #DeejayeyeHackingClub information repos aka "The OG's" (Original Gangsters)

http://dji.retroroms.info/ - "Wiki"

https://github.com/fvantienen/dji_rev - This repository contains tools for reverse engineering DJI product firmware images.

https://github.com/Bin4ry/deejayeye-modder - APK "tweaks" for settings & "mods" for additional / altered functionality

https://github.com/hdnes/pyduml - Assistant-less firmware pushes and DUMLHacks referred to as DUMBHerring when used with "fireworks.tar" from RedHerring. DJI silently changes Assistant? great... we will just stop using it.

https://github.com/MAVProxyUser/P0VsRedHerring - RedHerring, aka "July 4th Independence Day exploit", "FTPD directory transversal 0day", etc. (Requires Assistant). We all needed a public root exploit... why not burn some 0day?

https://github.com/MAVProxyUser/dji_system.bin - Current Archive of dji_system.bin files that compose firmware updates referenced by MD5 sum. These can be used to upgrade and downgrade, and root your I2, P4, Mavic, Spark, Goggles, and Mavic RC to your hearts content. (Use with pyduml or DUMLDore)

https://github.com/MAVProxyUser/firm_cache - Extracted contents of dji_system.bin, in the future will be used to mix and match pieces of firmware for custom upgrade files. This repo was previously private... it is now open.

https://github.com/MAVProxyUser/DUMLrub - Ruby port of PyDUML, and firmware cherry picking tool. Allows rolling of custom firmware images.

https://github.com/jezzab/DUMLdore - Even windows users need some love, so DUMLDore was created to help archive, and flash dji_system.bin files on windows platforms.

https://github.com/MAVProxyUser/DJI_ftpd_aes_unscramble - DJI has modified the GPL Busybox ftpd on Mavic, Spark, & Inspire 2 to include AES scrambling of downloaded files... this tool will reverse the scrambling

https://github.com/darksimpson/jdjitools - Java DJI Tools, a collection of various tools/snippets tied in one CLI shell-like application
