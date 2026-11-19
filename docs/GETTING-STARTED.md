# Getting started with Aperture

## Now Playing

Open **Settings → Now Playing** and select a source. **All Media** prioritizes playing Apple Music or Spotify when several sources are active. Swipe right inside the expanded player to cycle through available sources. In Duo, place your pointer over the player on the left.

Aperture can use media that macOS shares with third-party apps through Now Playing. Apple Music and Spotify have separate playback connections so they can stay available alongside a system session. The system menu can show sessions that macOS does not share with Aperture.

All Media keeps detected paused sources in the expanded player. When you pause or stop the current source, a source that is still playing can take over. If music and video are both playing, music appears first. You can still switch to the video.

Aperture also reads compatible visible browser players through its existing Device Control and Data Access permission. It reads the title and controls the browser exposes, including standard HTML video and supported custom players such as YouTube. Browser playback can offer Play and Pause when the page exposes them.

## Menu Bar

Open **Settings → Menu Bar** and turn on **Hide icons**. In **Auto**, Aperture checks the space the expanded island will need. With Auto off, eligible app icons start tucked away.

Click the arrow to reveal app icons. If optional controls were tucked too, the next click reveals them. Click again to tuck the items away, or set **Auto-hide after** to tuck them away automatically. The Aperture icon beside the arrow opens the app menu.

Automatic menu bar changes use the local Control Center settings folder and macOS menu bar geometry. Support for individual icons depends on how macOS registers them. Aperture excludes Live Activities, Wi‑Fi, Battery, and Control Center from its hiding rules.

## File Tray

Drag a file to the notch to open the tray, or swipe up over the island. Scroll sideways to see more files and hover over a tile to reveal its remove button. Removing a tile takes its shortcut out of Aperture. The file stays where you saved it.

## Appearance and Lock Screen

**Settings → General → Tuning** adjusts width and height by two display pixels in either direction. **Fit** is zero. The preview tracks the slider as you drag. Enable **Haptic feedback** to feel the steps on compatible trackpads.

Enable the playback and status widgets you want in **Settings → Lock Screen**. macOS supplies the clock. Aperture keeps the Lock Screen badges, including battery, off the screen saver. Focus badges and notifications remain available in their other views.

## Permissions and data

| Feature | Access |
| --- | --- |
| Calendar | Reads the calendars you connect to display events and reminders |
| Bluetooth | Reads device names and types for connection notifications |
| Music and Spotify | Uses Automation to read metadata and send playback controls when connected |
| Live waveform | Uses system audio to draw the waveform in memory |
| Menu bar and keyboard controls | Uses the macOS access requested by those options |
| Weather and time to leave | Uses your selected city for Open-Meteo and mapped events for Apple Maps |
| Updates | Checks the Aperture GitHub repository when you press Check for Updates |

Aperture’s private source and local development signing files are kept outside the release repository.
