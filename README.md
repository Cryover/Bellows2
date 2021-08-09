# Bellows - The lungs of the Foundry!
---

* **Author**: casualchameleon (discord: casualchameleon#6618)
* **Version**: 0.4.1 prerelease
* **Foundry VTT Compatibility**: 
  * 0.3.2 Tested on 0.6.6 and 0.7.5 
  * 0.4.1 Tested on 0.8.8 - **confirmed incompatible with 0.8.6**
* **System Compatibility (If applicable)**: n/a
* **Module Requirement(s)**: n/a
* **Module Conflicts**: Reported to conflict with Maestro - YMMV. It's plausible that any modules that change the playlist or ambient sound data could conflict with Bellows.
* **Translation Support**: Playlist import is localised at the moment, but nothing else. This is coming soon.

## Upgrading Bellows to Foundry 0.8+
If you have a previous installation of Bellows, then you'll need to reinstall the module as the manifest location has changed (sorry) - however, all your playlists and tracks will still work once the new version is installed.

## Link(s) to Module
* https://github.com/casualchameleon/Bellows
* https://github.com/casualchameleon/Bellows/releases/latest/download/module.json

## Description
This is a fork of temportalflux's fantastic [MusicAssist](https://github.com/temportalflux/MusicAssist) module which is no longer actively maintained. It aims to add support for youtube tracks and playlists, allowing users to grab their favorite youtube playlists and songs and save them as tracks in FVTT. These tracks are played back on each user's computer according to the normal playlist controls. This does require an internet connection to work properly, as it streams the video and just plays the audio.

Not all tracks and playlists are supported, as the YouTube author needs to enable embedding for Bellows to be able to play it.

## Installation
Import the [module.json](https://github.com/casualchameleon/Bellows/releases/latest/download/module.json) as you would any other module. The contents of the module directory should look similar to this github repository's root.

## Features

The current feature set includes:
- Playlist tracks can be imported from a youtube url such as `https://www.youtube.com/watch?v=_2xHCZSqpi4`
- Ambient Sound objects can be marked as streaming sounds with the same functionality as streamed playlist tracks (these are unable to fade however)
- YouTube Playlist imports

## Known Issues
- **Important** Importing high volumes of playlists can cause you to be temporarily timed out by the YouTube API as scraping songs from the iframe makes a lot of calls. Please only import what you need! If you do get timed out, cycling your IP address should fix it for you.
- In Firefox, audio may not play in certain scenarios due to autoplay restrictions. You can fix this by clicking the autoplay button in the url bar and allowing it for your Foundry VTT site. Each player using Firefox will need to do this for it to work. Chromium based browsers don't have this issue.

![image](https://user-images.githubusercontent.com/1485053/97107921-03e8ff80-16c2-11eb-8695-59da5c368a19.png)

## Credits
Massive thanks to [TemportalFlux](https://github.com/temportalflux) for his initial work on this project.

Thanks to [Blackcloud010](https://github.com/Blackcloud010) for his fantastic project template, [FoundryVTT-Module-Template-Hotswap](https://github.com/Blackcloud010/FoundryVTT-Module-Template-Hotswap).
