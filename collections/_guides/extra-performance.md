---
layout: guide
title: How to get Some Extra Performance from Diet Melee
---


*This guide is a work in progress. Join the discord and let us know if you have any feedback for it or think there’s anything else we should add to it!*

### Basic Slippi Dolphin settings to change:
	Config:
		Slippi:
			☐Save Slippi Replays
		Advanced:
			**☑Enable CPU Clock Override**
				**Set the slider to 80%. You can set this lower than 80%, some say as low as 40%. It’s worth experimenting with.**
	Graphics:
		General:
			**Backend: Direct3D 9(consider trying different backends, 9 is usually fastest but others might work better for your set up, definitely experiment with this)**
			**☐V-Sync**
			**☑Use Fullscreen**
		Enhancements:
			Internal Resolution: 1x (640x528)
			Anti-Aliasing: None
			Anisotropic Filtering: 1x

##### Also consider these tips:
Try deleting the contents in your <dolphin>/User/Cache folder. These are used by Dolphin for fast display calculations but if you recently changed your video card or updated drivers, it's possible these cached files will be out-of-date causing performance problems. After deleting this, make sure to play for at least 5 minutes before judging performance because Dolphin will need to re-process your cached shaders.

General computer speed up tips:

- ***If you’re on a laptop, make sure you’re plugged in and in the high performance battery setting.***
- **Close your browser**
- Close Steam
- Close Discord
- Press Windows > Settings > Apps > Start Up > And then turn off everything you don’t need. Then restart your computer.

### Force Simple Stage Geometry:

If after all of this you’re still having issues running Melee, try the Force Simple Stage Geometry gecko code. This tutorial’s screenshots are from a different guide but just use context clues to figure out what to put where.

[image]()

>[Gecko_Enabled]
>$Required: General Codes
>$Required: Slippi Recording
>$Required: Slippi Online
>$Recommended: Normal Lag Reduction
>$Recommended: Polling drift fix + VB
>-Optional: Widescreen 16:9
>-Optional: Disable Screen Shake
>-Optional: Center Align 2P HUD
>-Optional: Flash Red on Failed L-Cancel
>$HUD Transparency v1.1
>$Force Simple Background and Stage Geometry [Punkline]
>[Gecko]
>$Force Simple Background and Stage Geometry [Punkline]
>04028d64 60000010
>0405a2e8 60000000

1. Right click your vanilla iso
2. Select Properties
3. Click “Edit Config” in the bottom left corner of the properties window. This will open up GALE01.ini
4. Make sure you copy and paste the above text, so that your GALE01.ini looks something like this.
[image]()
5. File > save.
6. Close GALE01.ini
7. Click on “Gecko Codes” in the top middle of the properties window.
[image]()
8. Make sure it’s checked on.
9. Press close.
10. Start Melee, should be even better performance now.
