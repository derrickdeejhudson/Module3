## Introduction

The Oregon Trail series were a collection of educational games from the mid 1990's. It was designed to run on Windows 95 and will not run on windows 10. This is a guide to make this vintage classic game operate on modern Windows.

![Error on PC](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step1.png "You aren't on Windows '95")

## Installation instructions

### Requirements

- Windows
- Software to mount an .iso file
- Oregon Trail .iso file

I use [this](https://daemon-tools-lite.en.softonic.com/ "Daemon Tools Lite") but you may already have something that works. You can test by right clicking the a .iso file, if "mount" is an option then you already have what you need.

### Download

You can find it easily with a quick Google search, but [this](https://drive.google.com/file/d/1ZRpL7KFqrYPmRFTfEWE4R_iJDDDRlwTj/view?usp=sharing ".zip folder with .iso of Oregon Trail II") is the version used by this tutorial.

### Description of Equipment & List of Materials (with illustrations)

### Code example

This is what the contents of OREGONII.INI look like

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

### Example(s) of your code (if applicable)

### How to Contribute

![step2](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step2.png)

![step5](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step5.png)

![step8](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step8.png)
![step9](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step9.png)
![step10](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step10.png)

## FAQs

### Why do I just see a black screen?

It will go away, let it run for a few seconds think click. The window should open from there.

### Why isn't my sound working?

The music is muted by default, you can change that in the settings. Once you've turned music on you need to start an adventure then quit it to start hearing the main menu theme.

## Troubleshooting

If you are having trouble connecting to your directory, you can run the game from the mounted disc.
![step3](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step3.png)

You want to edit the OREGONII.INI

![step4](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step4.png)

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

Change the highlighted portion to the source of your BD-ROM Drive (E:) (or whatever yours is)
![step6](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step6.png)
![step7](https://raw.githubusercontent.com/derrickdeejhudson/Oregon-Trail-II/main/Images/step7.png)

## Licensing

Oregon Trail is considered abandonware. That is software that was made to be sold but is no longer being sold either online or in physical form by the original developer. In the case of Oregon Trail the software company that made many educational games, Softkey, has been out of business for over 20 years.

## Support

Create an [Issue](https://github.com/derrickdeejhudson/Oregon-Trail-II/issues)

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
