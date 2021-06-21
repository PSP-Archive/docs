# Guidelines for uploaders

Uploaders must be admins of the [PSP Homebrew Library](https://archive.org/details/psp-homebrew-library), otherwise it will not be possible to add their uploads to the collection (not even by the admins of the collection).

For your first few uploads, add your findings to the Open Data collection of the Internet Archive. This does not require you to be an admin of the PSP Homebrew Library, and you will be able to move the files into the collection once you are given the role.

## 'Not working' is relative

Nearly all apps and games that were published by major homebrew sites in the past do work on at least one firmware. And if developers decide to create updated custom firmwares, new apps might suddenly become 'working' or 'not working' as well. The definition depends entirely on the system's software.

To test, I decided to use neur0n's [LME custom firmware, version 6.61 - 2.3](https://archive.org/details/release_660lme.7z). This is because it supports Dark_Alex's Legacy Software Loader (aka [leda.prx](https://github.com/PSP-Archive/leda/releases)) - drastically boosting the number of apps that it can launch. Unfortunately, the same cannot be said of Pro or ARK at the moment.

## No flashers - ever

This is the cardinal rule. So many homebrews were created to add/remove assets from the system's NAND flash memory - to modify themes, add quality-of-life improvements or even simply to 'remove useless files'. 

Those are not welcome. In fact, if you don't want to say goodbye to your device, you'd better not test them at all.

The better flashers included checks for firmware versions and battery levels, but so many of them did not. Whatever they accomplished is largely irrelevant nowadays, and preserving them isn't worth the risk of causing someone's PSP to turn into a paperweight.

The handful of exceptions include apps that are actively used by most PSP users without issues - such as the latest versions of the Pro and LME custom firmwares. But that's about it. Everything else is to be deleted on sight.

## File structure

All homebrews must be compressed using the 7z format before uploading them.

The EBOOT file and its immediate contents must be placed at the root of the archive (as opposed to a subfolder). 

Add the usual memory stick structure to the archive *only if the homebrew requires it*. Example of this: the EBOOT that goes into the PSP/GAME folder, but to work it requires additional files at the root of the memory stick. [Monkey64](https://archive.org/details/monkey-64-0311.7z) shows how to deal with similar cases.

## Cover image

Any image uploaded in the root folder will be the cover image. Prefer in-game screenshots to artwork, menus or icons, as they provide a better impression of what the game looks like. 

For emulators, the better choice is to include a screenshot of the menu. Showing an emulated game would be less representative of the application in this case.

## Metadata structure

1. **Page Title**:
	1. Only include the name of the homebrew. Version numbers belong in their own field (see below).
1. **Subject Tags**:
	1. Pick one among 'game', 'application', 'emulator', 'demo'. Additional tags can be added where deeded relevant by the uploader (e.g. for genres, like 'shooter', 'visual novel', etc). 
	1. If a game participated in a competition (e.g. the NEO 2008 competition), add the relevant tag.
	1. **Support tags**:
		1. '1.50 FW only': if the game works on firmware 1.50, but not on any other version (even by using eLoader).
		1. 'PSP-2000+ only': if the game won't work on a PSP-1000 model.
		1. 'eLoader required': if the game won't boot without it.
		1. 'not working': if the game will not work on real hardware (on any firmware), but it is still retained for its historical value. This applies even if it does work on PPSSPP or another emulator.
	1. **Accessory tags**:
		1. 'Go!Cam': game supports or requires the PSP camera.
		1. 'Go!Explore': game supports or requires the GPS module.
		1. 'IrDA': game/app supports or requires an infrared device.
		1. 'Neo Motion Kit': unofficial motion kit accessory used by some homebrews.
	1. **Multiplayer tags**:
		1. 'ad-hoc support': game/emulator supports an ad-hoc multiplayer mode.
1. **Creator** field:
	1. Where both the real names and nicknames of a creator are known, prefer real names (as those tend to change less often).
	1. If the game/app is a port, enter the name of the creator of the PSP port. This is because the same game might have been ported several times by different people.
	1. If the number of creators is really large (more than 4-5) leave this field blank, and list them in the Description field instead.
1. **Date**:
	1. When main version of the game/app (i.e., the most recent one included in the item) was released. If the game/app was unreleased before being archived in the Homebrew Library, leave it blank. 
	1. All dates should be later than 2005-05-05 (when Nem released his Hello World for PSP).
	1. If the game/app is a port, enter the date when the port was released (so for DoomPSP it's 2006, not 1993).
1. **Language**:
	1. Only if a language other than English, leave blank otherwise. Only one language can be entered, so also leave it blank if multiple languages are supported. 
1. **License**:
	1. Only add if the game/app does mention a license within its content, and the license is available among the dropdown options - leave blank otherwise.
1. Additional metadata:
	1. **version**: Add a custom field named 'version' whenever a version number is available. This will make it easier to keep the most recent version as the main one. 
	- If multiple versions are available: add older versions in an "Old Versions" folder within the main item (as separate 7z files).
	1. **support-author**: a link to the PayPal, Patreon, Twitch or other payment page connected to the author of the homebrew. 
	
## Preview videos

Inclusion is completely arbitrary - adding them for every homebrew would require too much time.

Specifications:

- Must be under 1Mb, and about 10 seconds long.
- Audio: 64k AAC, mono
- Video: 600k AVC, PSP resolution (480x272)
