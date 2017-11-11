# Thymio workshop

Notes for [Crea Code Club](http://codeclub.heig-vd.ch/) [Thymio]() robot workshops for kids.

## Prep
* Install fresh version of [Aseba Studio](https://www.thymio.org/en:start)
* Max out Thymio volume. A loud Thymio is a fun Thymio. 
	1. Start or restart by pressing on middle button
	* Simultaneusly hold right and left arrow until robot turns red 
	* Press middle button while red
	* Use UP ARROW to max out volume

### Optional
Prepare a custom SD card with files to make a playable instrument using these [instructions](doc/createSoundFiles.md).

## Introduction
* Get them excited
	* Present Thymio: swiss robot made @EPFL by Francesco Mondada & team (sensors and default modes)
* Get to know their skills: ask about other workshops they took. Adapt difficulty.
* Explain differences between event-driven and sequential programming
* Show different robot modes
	*  Green = friendly: comes close
	*  Yellow = explorer: advances and avoids obstacles
	*  Red = fearful: avoids
	*  Cyan = investigator: follows black line
	*  Pink = obedient: control with direction buttons
	*  Blue = attentive: listen to claps 1x, 2x and 3x claps yield different results

## 01 Thymio Theremin
[<img src="https://s14-eu5.ixquick.com/cgi-bin/serveimage?url=https:%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F7%2F74%2FLev_Termen_playing_-_cropped.jpg&sp=e61486185f0cbeed477827774bbcae44">](https://en.wikipedia.org/wiki/Theremin)

[Léon Theremin Playing His Own Instrument](https://archive.org/details/LeonThereminPlayingHisOwnInstrument)

Create an instrument using the `Thymio VPL` software, like so.
Let them add extra actions on events.

![Instrument](img/00_instrument.png)

Using [Pitch analyzer](https://itunes.apple.com/us/app/pitch-analyzer/id571243369?mt=8) 
I reverse engineered the notes: 

![Instrument](img/01_sounds.png)

Here is a small melody by Gwen: 

```
c#4 c#4 E4 G4
E4  c#5 A4 G4
E4  c#4 A4
```

It should sound like [this](doc/GwenThymio.m4a).

## 01b Thymio tunes: Symphony No. 9 (Optional)
Since this does not use `VPL`, should probably be used as a demonstration.

* Load sounds from `/assets/sounds` onto SD card
* Insert SD card into Thymio and restart
* Load `00_playSDCardSounds.aesl` onto Thymio with `Aseba Studio`

Note | Count | Filename 
--- | --- | --- |
C | 1 | P0.wav
D | 2 | P1.wav
E | 3 | P2.wav
F | 4 | P3.wav
G | 5 | P4.wav

```
-------------------------------------
# Ode of joy
# E E F G   G F E D  C C D E  E D D
# 3 3 4 5   5 4 3 2  1 1 2 3  3 2 2
#
# E E F G  G F E D  C C D E   D C C
# 3 3 4 5  5 4 3 2  1 1 2 3   2 1 1
--------------------------------------
```

## 02 Basics
* Move forward
* Stop before frontal impact
* Avoid falling off the table
* Stop when hit and get angry
* Move in a circle
* Turn around itself
* Move towards the hand

## 03 Friendly behaviour

This already teaches them about motors. 
Should take some time to add animated behaviours.

They should get to the conclusion that with what they have they can not stop a collision. This is when we should introduce expert mode.

## 04 Line follower behaviour
1. Just follow lines.
* Handle traffic
* Avoid obstacles
* Stop if somebody in front

## 05 Police Siren or Sound of the police or Learning about State machines
Explain state machine with advanced mode and police siren. 


## 06 Poll booth

`todo: build rebuildable structure`

## Resources

[Intro Thymio video by Francesco Mondada](https://www.youtube.com/watch?v=QRyqZ0E5Ez0)


