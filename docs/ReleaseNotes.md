# Release Notes

## PiPedal 1.1.32

New features:

- 149 new ToobML presets

Bug fixes:

- Fix bypass not updating audio when triggering it with midi signal (https://github.com/rerdavies/pipedal/issues/146)
- Fix tuner not displaying the notes in the UI (issue was introduced in a commit that is not in the latest release)
- Fix white background in the banks managing screen in dark mode, making letter not legible
- Fix ToobML gain control not showing as disabled in the UI for presets that do not use gain (#3 )
- Fix some errors in docs and debug setup config

## PiPedal 1.1.31

- Use system preferences for dark mode when connecting from Android app.

## PiPedal 1.1.29

Bug fixes:

- TooB Convolution filenames not updating properly.


## PiPedal 1.1.28

New in this release.

- TooB Neural Amp Modeler - an LV2 port of  Steven Atkinson's astounding Neural Amp Modeler. Donwload model files from [ToneHunt.org](https://tonehunt.org). CPU is very high -- it runs on a Raspberry Pi 4 with just enough CPU left over for a couple of extra effects; but the results are worth it. TooB ML provides Neural Net modelled guitar amps with more modest CPU use (but considerably less flexibility).

- Dark mode. Go to the settings dialog to turn on Dark Mode. 

Bug fixes:

- Plugin information is updated in the web app after reconnecting, in order to pick up new plugins that may have been detected while the web server was being restarted.


## PiPedal 1.1.27

- Add missing lv2-dev dependency.

## PiPedal 1.1.26

- Revised file browser protocol for NAM and MODP plugin compatibility.
- Revised resource file publication extension.

## PiPedal 1.1.25

- New TooB BF-2 Flanger plugin
- New TooB Stereo Convolution Reverb

## PiPedal 1.1.24

- Reduce TooB Convolution Reverb and Toob Cab IR CPU use by 90%.

## PiPedal 1.1.23

Features:

-    Two new plugins: TooB Convolution Reverb, and TooB Cab IR.

-    Output ports for LV2 plugins are now displayed (vu meters and status controls)

-    File selection dialog, and uploads for LV2 atom:path Properties for 3rd party LV2 plugins.

Bug fixes:

-    Improvements to onboarding procedure.

-    Problems with restarting audio after changing audio parameters.

-    Occasional loss of audio after reboot caused by ALSA USB initialization race conditions.
