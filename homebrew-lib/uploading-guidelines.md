Uploaders must be admins of the PSP Homebrew Library, otherwise it will not be possible to add their uploads to the collection (not even by the admins of the collection).

## File structure

All homebrews must be compressed using the 7z format before uploading them.

The EBOOT file and its immediate contents must be placed at the root of the archive (as opposed to a subfolder).

## Metadata structure

1. Cover image:
	1. Any image uploaded in the root folder will be the cover image. Prefer in-game screenshots to artwork, menus or icons, as they provide a better impression of what the game looks like. 
1. **Page Title**:
	1. Only include the name of the homebrew. Version numbers belong in their own field (see below).
1. **Subject Tags**:
	1. Pick one among 'game', 'application', 'emulator', 'demo'. Additional tags can be added where deeded relevant by the uploader. 
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
1. **Creator** field:
	1. Where both the real names and nicknames of a creator are known, prefer real names (as those tend to change less often).
	1. If the game/app is a port, enter the name of the creator of the PSP port. This is because the same game might have been ported several times by different people.
1. **Date**:
	1. When main version of the game/app (i.e., the most recent one included in the item) was released. If the game/app was previously unreleased, leave it blank. 
	1. If the game/app is a port, enter the date when the port was released.
1. **Language**:
	1. Only if a language other than English, leave blank otherwise. Only one language can be entered, so also leave it blank if multiple languages are supported. 
1. **License**:
	1. Only add if the game/app does mention a license within its content, and the license is available among the dropdown options - leave blank otherwise.
1. Additional metadata:
	1. **version**: Add a custom field named 'version' whenever a version number is available. This will make it easier to keep the most recent version as the main one. 
	- If multiple versions are available: add older versions in an "Old Versions" folder within the main item (as separate 7z files).
	1. **support-author**: a link to the PayPal, Patreon, Twitch or other payment page connected to the author of the homebrew. 
