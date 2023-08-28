## League Director NG
[![Original License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://github.com/riotgames/leaguedirector/blob/master/LICENSE)
[![Python](https://img.shields.io/badge/python-3.10-brightgreen.svg)](https://www.python.org/downloads/release/python-372/)
[![Qt](https://img.shields.io/badge/pyside6-6.2.4-brightgreen.svg)](https://www.qt.io/qt-for-python)
[![Chat](https://img.shields.io/badge/chat-on%20discord-lightgrey.svg)](https://discord.com/invite/c2Qs9Y83hh)

League Director NG is a tool for staging videos from League of Legends replays. It is developed mainly to add extra features for creating in-game footage for the [League of Poro YT channel](https://www.youtube.com/@leagueofporo). This program builds on the original [League Director](https://github.com/riotgames/leaguedirector) developed by Riot Games.

![Screenshot](resources/screenshot.png)

## Features

* Control replay playback and speed
* First person camera controls
* Attach camera to champion or minion
* Toggle interface elements including HUD, health bars and notifications
* Graphical Options
  - Field of view
  - Near and far clipping
  - Custom skyboxes
  - Shadow direction
  - Depth and height fog
  - Depth of field
* Sequencer
  - Record and playback keyframed camera position + graphical options
  - Timeline for viewing and editing keyframe values
  - Undo / Redo
  - Save and load pre saved sequences
  - Adjustable keyframe blending
* Customizable key bindings

## TO DO
- ~~Hover line that shows the time on the sequence~~
- Drag select and move multiple keyframes
- Copy and paste keyframes
- New keyframes - snap-snap, linear-snap, snap-linear (to address the unwanted persistence of movement)
- Fit curve to linear keyframes to avoid choppy cuts

## How To Use

**Note: Windows Only**

1. **Download League Director** from the releases page and install.
2. Start League Director and make sure the checkbox next to your install is checked.
3. Start League of Legends and launch a replay. League Director will automatically connect.
4. Open the options menu (ESC key) in game and ensure your Video Graphics settings are set to Very High. If you did need to change your Video Graphics settings, you'll need to restart the replay to enable the additional rendering features like the skybox.
5. Select FPS Camera from the Camera Modes drop down in game.
6. Using the numpad keys (4, 5, 6, 8) and the mouse you can free camera move around. Key bindings for free camera can also be changed inside the game options.

## Tutorials
Introduction | Walkthrough
------------ | -------------
[![](http://img.youtube.com/vi/bzqydcrw89A/0.jpg)](https://www.youtube.com/watch?v=bzqydcrw89A "League Director Intro")|[![](http://img.youtube.com/vi/KuHLaDRReRU/0.jpg)](https://www.youtube.com/watch?v=KuHLaDRReRU "League Director Tutorial")

## Frequently Asked Questions
**How do I change the keybindings for camera movement?**

The forward, back, left, right key bindings for the FPS camera are actually set in the game options screen. With a replay running, open the options screen (ESC) and then go into 'Hotkeys' and into the section 'First Person Camera'.

**Why is the skybox black?**  
**Why won't the skybox change?**

League Director requires your game to be set to the highest graphics settings. With a replay running, open the options screen (ESC) and under the 'Video' section set the graphics options to 'Very High'. You must restart the replay after changing this setting in order for it to take effect.

**League Director does not show my game install on the options screen?**  
**League Director does not connect to my replay?**

If league director fails to find and configure your game client correctly don't worry because you can do it manually. Simple open up an explorer window where to where your game is installed, then look inside the Config folder for a file called 'game.cfg'. Right click and open this file with notepad and under the section labeled '[General]' make sure there is a value set to the following.

```
EnableReplayApi=1
```

If the option is already listed make sure it is set to 1. If the option is not listed at all just add it to the bottom of the list. You will need to restart the replay after changing this value for it to take effect.

## License
Apache 2 (see [LICENSE](https://github.com/riotgames/leaguedirector/blob/master/LICENSE) for details)

For usage rights of Riot Games intellectual property, such as the skybox textures bundled with this installer, please refer to:

[https://www.riotgames.com/en/legal](https://www.riotgames.com/en/legal)

This project makes used of LGPL licensed software [QT for Python](https://doc.qt.io/qtforpython/licenses.html).

## Special Thanks
 * Skin Spotlights
 * League of Editing
