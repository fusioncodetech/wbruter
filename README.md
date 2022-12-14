# WBRUTER

#### README

wbruter is is the first tool wich has been released as open source wich can guarantee **100%** that your pin code will be cracked aslong as usb debugging has been enable. wbruter also includes some other brute methods like dictionary attacks for gmail, ftp, rar, zip and some other file extensions. 

wbruter will allways try to bring support for rare protocols, wbruter wont contain common stuff like other brute tools cover like facebook, snapchat, instagram and you name it (except a few exceptions, very few)

_Many times it's the easiest methods that are the most powerful methods, it's just a matter of using your imagination ;-)_


## INFO: 2020-07-11:

Android and Google, now have set a rule for locksettings via cli as via gui earlier, if you try to many attempts within X seconds you will be blocked for X seconds so wbruter via cli wont work anymore on devices that has been upgraded to latest version Android 10, older version should work fine unless they are upgraded to latest android version. 

## Enable USB-Debugging via the methods below:

#### Via GUI: 

Go to settings -> about > press on build number 7 times and the developer settings will be enable, go back to settings and press on developer mode and then enable USB DEBUGGING. If you found an android deviceon the street or something and want to break the pin this wont be possible unless you already know the pin so the device must have usb debugging enable for this to work. You wanna try this for fun then you can just enable usb debugging after you unlocked phone)

#### Via cli/adb: 

     settings put global development_settings_enabled 1
     setprop persist.service.adb.enable 1

#### Via GUI (old layout now use --androidgui 4 instead)
##### Please use cli method instead since many devices has been set to erase the device after "10/15 wrong pin attempts" and this wont happen with the CLI method. (Updated: Jan/2019)

![Screenshot](https://raw.githubusercontent.com/1939149/wbruter/master/files/wbruter.gif)

#### Via CLI:

From 0000 to 9999 takes ~83 minutes. In around ~1h you will with 100% _guarantee_ have the pin code

![Screenshot](https://nr1.nu/archive/wbruter/previews/wbruter-cli.gif)

#### Notice:

If you will see a message similiar to message under you don't have to care, just let it run and it will be gone after ~4-5 failed attempts: 

      Error while executing command: clear
        java.lang.RuntimeException: No data directory found for package android
        at android.app.ContextImpl.getDataDir(ContextImpl.java:2418)
        at android.app.ContextImpl.getPreferencesDir(ContextImpl.java:533)
        at android.app.ContextImpl.getSharedPreferencesPath(ContextImpl.java:795)
        at android.app.ContextImpl.getSharedPreferences(ContextImpl.java:394)
        at com.android.internal.widget.LockPatternUtils.monitorCheckPassword(LockPatternUtils.java:1814)
        at com.android.internal.widget.LockPatternUtils.checkCredential(LockPatternUtils.java:398)
        at com.android.internal.widget.LockPatternUtils.checkPassword(LockPatternUtils.java:548)
        at com.android.internal.widget.LockPatternUtils.checkPassword(LockPatternUtils.java:509)
        at com.android.server.LockSettingsShellCommand.checkCredential(LockSettingsShellCommand.java:151)
        at com.android.server.LockSettingsShellCommand.onCommand(LockSettingsShellCommand.java:57)
        at android.os.ShellCommand.exec(ShellCommand.java:96)
        at com.android.server.LockSettingsService.onShellCommand(LockSettingsService.java:1945)
        at android.os.Binder.shellCommand(Binder.java:574)
        at android.os.Binder.onTransact(Binder.java:474)
        at com.android.internal.widget.ILockSettings$Stub.onTransact(ILockSettings.java:419)
        at com.android.server.HwLockSettingsService.onTransact(HwLockSettingsService.java:179)
        at android.os.Binder.execTransact(Binder.java:675)


#### HOW TO

    git clone https://github.com/fusioncodetech/wbruter
    cd WBRUTER; ./wbruter --help

#### REQUIREMENTS

1. Termux App
2. ADB for Termux- Copy the Code Below and Paste on Termux APP

          apt update && apt install wget && wget https://github.com/MasterDevX/Termux-ADB/raw/master/InstallTools.sh && bash InstallTools.sh
          
3. Github Source Code..

#### USAGE

1.  Open Termux App
2.  Install ADB Packages

          apt update && apt install wget && wget https://github.com/MasterDevX/Termux-ADB/raw/master/InstallTools.sh && bash InstallTools.sh
          
3.  Install Git Packages

          pkg install git
          
4.  Install our Source Code

          git clone https://github.com/fusioncodetech/wbruter.git
          
5.  Go Installation Directory

          cd wbruter
          
6.  Set Root Permission

          chmod +x *
          
7.  Run wbruter

          ./wbruter
          ./wbruter --android
          ./wbruter --android 4
          ./wbruter --android 6
          
Note: Before run this tool you need to connect locked android device by OTG to your phone..

#### CONTACT 

If you have problems, questions, ideas or suggestions please contact me by posting to @fusioncodetech

#### WEB SITE

Visit my websites and profiles for the latest info and updated tools

https://unlockertools.blogspot.com

#### END!
