# Andoukie2 (doukie client for Android. Version 2!)

doukie2 client for Android. ([what is doukie2? here](https://github.com/yasutakatou/doukie2).)

# attention!

this repository is [not compatible previous version](https://github.com/yasutakatou/doukie).<br>
If you use to this repository, **you can't use previous version**.<br>
[Android client](https://github.com/yasutakatou/andoukie) **can't use previous, too**.<br>

## this version support additional features following.

- **recursive folder copy**.
- **save options to file when exit**.
- **sync progress is display**.
- **HTTPS support**.

# demo

![andoukie](https://github.com/yasutakatou/andoukie/blob/pic/andoukie.gif)

# solution

**AirDrop**, **Nearby Share** is very useful file transfer method.<br>
<br>
But, It's not what I'd expect opened economy method.<br>
<br>
Only use between Android. <br>
or on not supported computers, is require support by official or OSS comunity effort.<br>
<br>
**We know universal protocol, is HTTP.**<br>
<br>
I think to want implement easy file transfer method by HTTP.<br>
and, I realize file transfer on multi platform **(include Smart phone!)**.

# features

 - **read QR Code to syncing (no input operation)**
 - **gauge and switch easily operation**
 - file exists check (use md5 hash)
 - recursive folder copy.
 - save options to file when exit.
 - sync progress is display.
 - HTTPS support.

# installation

manually install

```
git clone https://github.com/yasutakatou/andoukie2
cd andoukie2
cordova platform add android
cordova build android
(displaying place of adb file.)
adb install (place of adb file.)
```

[or download binary from release page](https://github.com/yasutakatou/andoukie2/releases).<br>
save binary file, and adb install.

```
adb install (place of adb file.)
```

# uninstall

use app uninstall method on Android.

# method of operation

 - 1st

![1](https://github.com/yasutakatou/andoukie/blob/pic/1.png)

run doukie2 on you want to sync device.<br>
after running, enter key or space key on terminal console.<br>
QR Code displaying.<br>
run this app on Android, and read to QR Code.<br>

 - 2nd

operating on Android touch pannel.<br>

![2](https://github.com/yasutakatou/andoukie/blob/pic/2.png)

① not delete mode

default this switch is off.<br>
If some file exists Android, but not exists server, that file delete on .<br>
**when turn on this switch to not delete**.<br>

② gauge of sync interval

this gauge is interval of file syncing.<br>
**example (60), is sync every 60 seconds.**<br>
**(0) is not syncing.**<br>

③ status column

This place display sync status or another message.<br>

# problem

- fail to large file download!

this tools  download little by little implement, <br>
therefore The short sync cycle interrupt download session at larger file.<br>
So,you operate **"gauge of sync" longer**.<br>

- why Android can't use server and auto sync mode?<br>

this application builed by Apache Cordova.<br>
Cordova plugins are very instability.<br>
I can't work to want any features.<br>
**(I feel about 50% not work. because depend old Android API.)**<br>
By the next try to build Android application, I consider another framework, react native, Flutter..<br>

# FYI (many thanks!)

 - gauge for sync duration<br>
https://github.com/andrepxx/pure-knob

 - save blog data to binary file<br>
https://ourcodeworld.com/articles/read/230/how-to-save-a-pdf-from-a-base64-string-on-the-device-with-cordova

 - file remove<br>
https://stackoverflow.com/questions/33752990/cordova-remove-file

 - get file list<br>
https://gist.github.com/bcabanes/14e6d3221b841bfdf27b

# LICENSE

Apache License, Version 2.0

