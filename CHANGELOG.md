### CHANGELOG FOR WBRUTER

##### Version 2.1.0

-    Removed the ascii art from WBRUTER so we can have a better help section without things will be a mess
-    Cleaned up entire code to be much more readable for new users
-    Added a unique method for brute force attacking ssh connections, from now we using PARALLEL SSH for this (pssh)
-    Changed so we using IF for read variables instead of getopts, there is now 4 examples of executing every command
     + -X
     + -XOPTION
     + --X
     + --XOPTION
-    Added support for break ZNC bouncers web gui passhrases (https://imgur.com/a/O6mZDyJ)
-    Added support for brute force android devices that has been protected by a passworda via locksettings, 
     + WBRUTER is the first public release that using this method that can guarantee the pin will be breaked without any riskes for data loss aslong as usb debugging has been enable.

#### Version 2.0

-    Added support for break GPG encrypted files that has been protected by a password
-    Added support for break FTP credenticals that wich is protected by a password, username is required to figure out yourself (usually admin, root, guest, support is added)
-    Added support for break ZIP encrypted files that has been protected by a password
-    Added support for break RAR encrypted files that has been protected by a password
-    Added support for brute force android devices that has been protected by 6 digits via GUI Screen, we use swipe and touch screen for this by ADB
-    Added support for brute force android devices that has been protected by 4 digits via via locksettings
     + WBRUTER is the first public release that using this method that can guarantee the pin will be breaked without any riskes for data loss aslong as usb debugging has been enable.
-    Added support for brute force android devices that has been protected by 6 digits via via locksettings
     + WBRUTER is the first public release that using this method that can guarantee the pin will be breaked without any riskes for data loss aslong as usb debugging has been enable.

#### Version 1.0

-    WBRUTER has support for brute force android devices that has been protected by 4 digits via GUI Screen, we use swipe and touch screen for this by ADB
-    WBRUTER has support for brute force attacking GMAIL accounts.
-    WBRUTER has been released.

