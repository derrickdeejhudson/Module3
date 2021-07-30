## Introduction

The Oregon Trail series were a collection of educational games from the mid 1990's. It was designed to run on Windows 95 and will not by default run on windows 10. This is a guide to make this vintage classic game operate on modern Windows.

![Error on PC](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step1.png "You aren't on Windows '95")

### Requirements

- Windows
- Software to mount an .iso file
- Oregon Trail .iso file

## Tools

I use [this](https://daemon-tools-lite.en.softonic.com/ "Daemon Tools Lite") but you may already have something that works. You can test by right clicking the a .iso file, if "mount" is an option then you already have what you need.

![Mount](https://www.windowscentral.com/sites/wpcentral.com/files/styles/xlarge/public/field/image/2020/11/file-explorer-context-menu-mount-option.jpg)

### Download

You can find it easily with a quick Google search, but [this](https://drive.google.com/file/d/1ZRpL7KFqrYPmRFTfEWE4R_iJDDDRlwTj/view?usp=sharing ".zip folder with .iso of Oregon Trail II") is the version used by this tutorial.

## Installation instructions

1. Navigate to E:\Data in Windows Explorer and copy only the selected files into a new Folder, I named mine "OT2".

![step2](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step2.png)

If you try to run the OTII32.EXE executable you will see this error.

![step3](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step3.png)

2. Edit the OREGONII.INI file

![step4](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step4.png)

## Code example

The contents of which look like this.

```
[Sound]
music=on
sfx=on
speech=on
buffers=20,2000

[cdrom]
rsrcpath=d:\data
intromovieid=100


speed=1
[game]
speed=1

```

3. Change the highlighted portion to the source of CD drive.

![step6](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step6.png)

Mine is BD-ROM Drive (E:), yours may be different. Use the appropriate source for your disk drive.

![step7](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step7.png)

### Eureka!

Now you are able to play from the mounted disc! However we can do better, we can make the game run without the disc having to be mounted.

4. Into the same destination folder from step 1, copy over the remaining files.

![step8](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step8.png)

again, I named folder OT2

![step9](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step9.png)

where we saw d:\data originally

```
[cdrom]
rsrcpath=d:\data
intromovieid=100
```

and changed to e:

```
[cdrom]
rsrcpath=d:\data
intromovieid=100
```

5. we now want to set to the destination path of the folder you made.

## Code example

This is what the contents of OREGONII.INI look like on my machine.

```
[Sound]
music=on
sfx=on
speech=on
buffers=20,2000

[cdrom]
rsrcpath=C:\Users\DEEJ\Desktop\OT2
intromovieid=100


speed=1
[game]
speed=1

```

### How to Contribute

![step5](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step5.png)

![step10](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step10.png)

## Troubleshooting

If you are having trouble connecting to your directory, you can run the game from the disc.
![step3](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step3.png)

You want to edit the OREGONII.INI

![step4](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step4.png)

The contents of which look like this.

```
[Sound]
music=on
sfx=on
speech=on
buffers=20,2000

[cdrom]
rsrcpath=d:\data
intromovieid=100


speed=1
[game]
speed=1

```

Change the highlighted portion to the source of CD drive.

![step6](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step6.png)

Mine is BD-ROM Drive (E:)

![step7](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step7.png)

## FAQs

### Why do I just see a black screen?

It will go away, let it run for a few seconds think click. The window should open from there.

### Why isn't my sound working?

The music is muted by default, you can change that in the settings. Once you've turned music on you need to start an adventure then quit it to start hearing the main menu theme.

## Licensing

Oregon Trail is considered abandonware. That is software that was made to be sold but is no longer being sold either online or in physical form by the original developer. In the case of Oregon Trail the software company that made many educational games, Softkey, has been out of business for over 20 years.

## Support

Create an [Issue](https://github.com/derrickdeejhudson/Oregon-Trail-II/issues)
