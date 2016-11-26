# qq-translation

**Translates Tencent QQ into English (This is not QQ International)**

I recently discovered that Tencent bundles its QQ binaries into an exe file which could be extracted by commonly used unzipping tools. Moreover the archive doesn't feature any cert stuff.

Files and folders the archive contains include:

```
Folder PATH listing for volume Windows20_OS
Volume serial number is BA83-D081
C:\USERS\DUO\DOWNLOADS\QQ7.9LIGHT
├───Application Data
│   └───Tencent
│       └───QQ
│           ├───Misc
│           │   └───ClientType
│           ├───QQApp
│           │   └───100001
│           ├───SafeBase
│           └───Skins
│               └───system
│                   ├───1.45_16
│                   ├───1.45_17
│                   ├───1.45_18
│                   ├───1.45_19
│                   ├───1.45_20
│                   ├───1.45_21
│                   ├───1.45_22
│                   ├───1.45_23
│                   ├───1.45_24
│                   ├───1.45_25
│                   ├───1.45_26
│                   ├───1.45_27
│                   ├───1.45_28
│                   └───1.45_29
├───Common
│   └───Tencent
│       ├───Npchrome
│       └───TXFTN
└───Files
    ├───AuI18N
    │   └───2052
    ├───Bin
    │   ├───LICENSE
    │   └───plugins
    ├───I18N
    │   └───2052
    ├───Misc
    │   ├───BrSelfExp
    │   │   └───2052
    │   ├───CSC
    │   │   └───2052
    │   │       ├───1
    │   │       ├───10
    │   │       ├───11
    │   │       ├───13
    │   │       ├───14
    │   │       ├───15
    │   │       ├───2
    │   │       ├───3
    │   │       ├───4
    │   │       ├───5
    │   │       ├───7
    │   │       ├───8
    │   │       └───9
    │   ├───Editor
    │   │   ├───css
    │   │   ├───html
    │   │   │   └───css
    │   │   ├───images
    │   │   │   └───newicon
    │   │   └───release
    │   ├───LNNEsc
    │   │   └───defaultTips
    │   ├───QQApp
    │   ├───QScan
    │   └───Sound
    │       └───Classic
    ├───Plugin
    │   ├───Com.Tencent.AudioVideo
    │   │   ├───bin
    │   │   └───Misc
    │   ├───Com.Tencent.CRM
    │   │   ├───Bin
    │   │   └───Misc
    │   │       └───html_template
    │   │           └───img
    │   ├───Com.Tencent.DingDong
    │   │   └───Bin
    │   ├───Com.Tencent.FileTransfer
    │   │   └───Bin
    │   ├───Com.Tencent.Mail
    │   │   └───Bin
    │   ├───Com.Tencent.NetDisk
    │   │   └───Bin
    │   │       └───QQDisk
    │   │           └───Bin
    │   ├───Com.Tencent.QQVip
    │   │   ├───Bin
    │   │   └───Misc
    │   │       ├───CustomFont
    │   │       │   ├───101
    │   │       │   ├───102
    │   │       │   ├───103
    │   │       │   └───104
    │   │       └───supervip
    │   ├───Com.Tencent.Qzone
    │   │   ├───Bin
    │   │   ├───FlashPlayer
    │   │   │   └───I18N
    │   │   │       └───2052
    │   │   └───Misc
    │   │       └───qzonepackage
    │   ├───Com.Tencent.RemoteControl
    │   │   └───Bin
    │   ├───Com.Tencent.RemoteHelp
    │   │   ├───Bin
    │   │   └───Misc
    │   ├───Com.Tencent.SNSApp
    │   │   └───Bin
    │   └───Com.Tencent.Wireless
    │       └───Bin
    ├───Resource.7.9.14308
    │   └───Themes
    └───ShellExt
```

The archive is a QQ 7.9 Light version, which could be obtained from <http://im.qq.com>.

MD5 checksum: 1ccc5df82e68c2f5028379dec0a047c1

You are looking for the XML config files inside the I18N folders, which are translations for respective components.

There are also some config files pointing to different folders that store different language files, for example the 2052 folder is for Chinese (Simplified).

The config file declares many languages, each with a unique ID that is consistent with the numbered folders I said above.

This is really an interesting thing...

There will be a wiki (perhaps?) telling how to translate, switch between languages as well as how to re-bundle the translated files as a new executable for easy installation.
