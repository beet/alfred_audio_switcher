# Alfred Audio Switcher

Alfred workflow to quickly switch between audio **output** devices.

![pic](images/icon.png)

**Credit:** [Switch Audio Input/Output Device using Alfred – AgileAdam.com](https://agileadam.com/2020/05/switch-audio-input-output-device-using-alfred/) for the idea, I've just made some icons and packaged it up.

## ⚠️ IMPORTANT ⚠️: install `switchaudiosource`

For this to you work, you need to use [Homebrew](https://brew.sh/) to install `switchaudiosource`:

```bash
brew install switchaudio-osx
```

## Switching between audio devices

Provides keyword inputs to quickly switch between headphones, speakers, and an external device:

| Device           | Keyword |
| ---------------- | ------- |
| Headphones       | `ash`   |
| Speakers         | `asp`   |
| External         | `asx`   |

The first time each is used, it will prompt you to select the audio source for that device and then save it for next time _(which may take a few seconds to take affect)_. The next time it should switch to that device immediately.

**NOTE:** the macOS multimedia volume controls don't don't seem to affect the volume of external audio devices.

### Changing saved audio devices

Once you've switched to an audio device and it has been saved, if you want to change it to a different device, click the `[X]` icon in the top right of the workflow settings to access the Workflow Environment Variants, and delete the value.

Then when using the relevant keyword for that device next time, it should prompt you to select it again and save it.

## Select audio source

* Keyword: `asel`

Can use this at any time to present a list of _all_ audio devices currently connected to your system:

![pic](images/select_audio_device.png)

Does not save the selected value.
