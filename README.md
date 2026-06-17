# Night Display

A calm fullscreen night clock for Discord calls, late-night study sessions, and sleepy screen sharing.

Night Display shows a large glowing clock over a cozy blue lofi-style room scene, with an away message, friend time zones, dimming controls, and generated ambient sleep sounds. It is designed to be readable in the dark without feeling harsh on the eyes.

## Features

- Large elegant clock with optional seconds
- Cozy animated blue night-room background
- Away status message for friends on call
- Friend clocks for Sydney, Perth, and London
- Brightness dimmer for dark rooms
- Fullscreen mode
- Theme swatches
- Optional date display
- Generated ambient sounds: Waves, Rain, Hush, and Dream pad
- Settings saved in the browser
- No install step or external assets required

## How to Use

Open `index.html` in a browser.

For Discord, share the browser window, click the fullscreen button, choose a sound if you want one, then let the controls fade away.

Browsers require a click before audio can start, so press the play button once after opening the page.

## Running Locally

You can open the file directly, or serve it locally:

```bash
python3 -m http.server 4173
```

Then open:

```text
http://localhost:4173
```

## Customizing

The app is currently a single `index.html` file. You can edit:

- The away message from the on-screen input
- The friend clocks in the `friendClocks` array
- The theme colors in the CSS theme classes
- The ambient sound options in the audio engine

## Notes

The background is inspired by cozy lofi room and focus-session apps, but all visuals are built with HTML, CSS, and Canvas.

Audio is synthesized live in the browser. No music files are included.
