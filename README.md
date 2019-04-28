# sup1hdaudio
Fix for TempleOS Intel HD Audio driver (Written by Terry A. Davis)

This is a fix for the Intel HD Audio driver on the TempleOS Supplemental Disc #1. Tested, working on real hardware.

# Usage

Copy files over your existing ~/Sup1 directory, and add the following to Once.HC.Z (or other startup script):

```
	Cd("~/Sup1/Sup1Snd");
	AdamFile("MakeSnd");
	Cd("~Sup1/Sup1HDAudio");
	AdamFile("HDAudio");
```

You can set mixer settings using the following program:

```
	Cd("~/Sup1/Sup1HDAudio");
	#include "HDCfg";
```