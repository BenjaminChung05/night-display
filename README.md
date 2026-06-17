# Night Display

A calm fullscreen night clock for Discord calls, late-night study sessions, and sleepy screen sharing.

Night Display shows a large glowing clock over a cozy blue lofi-style room scene, with an away message, friend time zones, dimming controls, and generated ambient sleep sounds. It is designed to be readable in the dark without feeling harsh on the eyes.

## Features

- Large elegant clock with optional seconds
- Cozy animated blue night-room background
- Away status message for friends on call
- Customizable friend clocks with add/remove timezone slots
- Brightness dimmer for dark rooms
- Fullscreen mode
- Theme swatches
- Built-in still and live background library
- Custom photo, GIF, or video background
- Optional date display
- Generated ambient sounds: Waves, Rain, Hush, and Dream pad
- Settings saved in the browser
- No install step or external assets required

## How to Use

Open `index.html` in a browser.

For Discord, share the browser window, click the fullscreen button, choose a sound if you want one, then let the controls fade away.

Browsers require a click before audio can start, so press the play button once after opening the page.

Use the `bg` button to choose a local image, GIF, or video background. The file is stored in that browser only and can be removed with `reset`.

Use the background dropdown to choose from the built-in library: the original lofi room, still scenes, and live animated scenes. If you upload your own background, it appears as `My upload` in that same library.

Use the timezone row to choose which country or city clocks appear. The `+` button adds another clock, and each `-` button removes one.

## Running Locally

You can open the file directly, or serve it locally:

```bash
python3 -m http.server 4173
```

Then open:

```text
http://localhost:4173
```

## Publishing

This is a static site, so pushing `index.html` to GitHub makes the source available, but visitors need a hosted URL to use it easily. Netlify can publish straight from the GitHub repo; after you push changes, trigger a new deploy or let Netlify auto-deploy from the connected branch.

The status message, toggles, chosen timezones, chosen library background, and custom background stay in each visitor's own browser storage. The app does not send those choices to GitHub, Netlify, or a shared server.

## Customizing

The app is currently a single `index.html` file. You can edit:

- The away message from the on-screen input
- The default friend clocks in the `defaultWorldClocks` array
- The available timezone choices in the `timezoneLibrary` array
- The theme colors in the CSS theme classes
- The ambient sound options in the audio engine

## Notes

The background is inspired by cozy lofi room and focus-session apps, but all visuals are built with HTML, CSS, and Canvas.

Audio is synthesized live in the browser. No music files are included.
