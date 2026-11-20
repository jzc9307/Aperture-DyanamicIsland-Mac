# Getting started with Aperture

This guide covers the current interface. **v0.2.0 is unreleased**; Up Next, AirDrop activity and screenshot-drop improvements described here are development-preview features. See the [version notes](releases/v0.2.0.md).

## Install and open Settings

Open the downloaded DMG, drag **Aperture** into **Applications**, and launch it. Use the Aperture menu or right-click the island to open **Settings**. Choose your display and preferred idle activity in Settings. Apple silicon and macOS 15+ are required; native Liquid Glass appearance requires macOS 26+.

Click the compact island to expand it. Move the pointer away to let an unpinned activity close. Hover-to-expand is a separate option: when enabled, it waits for your selected hover delay before opening the full panel. The small pointer feedback does not require full hover expansion.

## Music sources and controls

In **Settings → Now Playing**, select **Apple Music**, **Spotify**, **Automatic · System**, or **All Media**. Connect the selected player when requested. All Media combines detected sources and gives playing music priority when several sources are active.

Swipe right over the expanded player to cycle available sources. In Duo, place the pointer over the music panel on the left. Paused detected sessions remain available in the expanded player; compact artwork hides after your **Idle duration**. Another source that is still playing can take over.

Use the seek bar to change playback position, and use the output icon to show or hide inline volume. Favorite is an Apple Music action. The extra button can instead show Shuffle, Repeat or Copy. Supported controls depend on the selected source and audio output.

Compatible browser players are read through the app’s Device Control and Data Access permission when their playback details and controls are exposed. Standard HTML media and supported custom players can work, but not every page or system session is available to Aperture.

### Live waveform

Turn on **Use live waveform** and approve system-audio access if macOS requests it. The live glyph follows six frequency bands from the system output; compact, expanded and Lock Screen music views use that same signal. Audio stays in memory and is not saved as a recording.

Turn the option off to use the decorative playback animation. If live mode is selected but the audio service is unavailable, it does not silently substitute decorative motion. Check the status message beneath the settings card.

### Up Next · v0.2.0

1. Play a song in Apple Music and open Music’s **Playing Next** sidebar.
2. Enable **Up Next peek** in Aperture’s Now Playing settings.
3. Set **Show Up Next before end** between **2 and 10 seconds**. New settings default to **5 seconds**.
4. Near the end, the compact island shows the next track and countdown when current queue data is available.

The sidebar must remain exposed. Repeat-one, paused playback and stale queue information suppress the peek. Aperture does not infer the next track from playlist order. Artwork is matched from local Music metadata or Apple’s catalogue; private/local tracks and unmatched editions may have no cover.

**Quick Peek** is different: it briefly shows information when the current track changes. Its **Peek duration** setting does not change the Up Next countdown.

## Lock Screen music and status widgets

Open **Settings → Lock Screen** and enable the lock presentation and **Now Playing widget**. Aperture’s separate floating music player shows:

- Album artwork, song title, artist and a live/decorative waveform according to your setting.
- Elapsed/remaining time and a seek bar for compatible sources.
- Shuffle, previous, play/pause and next controls.
- An indicator for the current audio output.
- A volume slider when **Show volume control** is enabled and the device supports adjustment.

Choose **Glass** or **Clear**, set how long a paused track remains visible with **Idle duration**, and move the player using **Vertical offset**. Appearance depends on macOS and the wallpaper; native Liquid Glass is available on macOS 26+.

The smaller status widgets are configured separately. Choose battery, connected devices, Focus and Calendar. Weather has its own switch and requires a selected city. Use **Widget order** to rearrange the status row.

**Show on screen saver** allows the lock presentation during the screen saver. Status badges hide while the screen saver is active. Lock/unlock sounds and the keep-awake duration are optional. Widgets dismiss on unlock, followed by the notch’s unlock animation.

The system clock and authentication belong to macOS. Aperture adds widgets rather than replacing the Lock Screen. Animated Apple Music album artwork is not currently included.

## Calendar and Duo

Connect Calendar when prompted, then select which calendars and display modes you want. Calendar shows today’s date and events on one side and upcoming days in its scrolling agenda. Event cards open the corresponding event.

Enable the month-view option for a calendar grid and optionally show event indicators. Reminder lead time and Quick Peek settings control when event information appears. **Duo** places music controls beside today’s schedule.

For mapped events, the optional time-to-leave feature uses Apple Maps, your transport choice and travel buffer. Empty-day weather requires weather to be enabled and a city selected.

## File Tray

Drag a file toward the notch, use **+** in the tray, or swipe up over the island. Scroll sideways through the items. Double-click a tile to open it; drag it out into a compatible app or Finder folder. Hover to reveal the remove button. Swipe down to return to activities.

Removing a tile removes the tray entry, not the original file. In v0.2.0, dragging the floating screenshot thumbnail or a temporary image stores a retained copy under Aperture’s local Application Support storage. That copy keeps the tray item available after the original temporary file disappears. Import errors appear in the tray.

### Sending and receiving AirDrop · v0.2.0

Use the tray’s AirDrop button to send its files, or use **Settings → AirDrop → Choose Files**. Choose a recipient in macOS. Set **Expand while sending** and **Expand while receiving** independently.

Accept or decline incoming requests in the **native macOS prompt**. Aperture does not replace it or suppress the native completion notification. A received preview is available after import. The activity ring is not a measured transfer percentage.

## Menu Bar

Enable **Hide app icons** in **Settings → Menu Bar**. **Only when space is tight** checks the room needed by the expanded island. Turn it off to start with eligible icons tucked away. Enable **Include Siri, Now Playing & Text Input** to include eligible optional controls as a second group.

Click the arrow to reveal app icons. If a second group is hidden, the next click reveals that group. Click again after the last reveal to tuck everything away. **Auto-hide after** controls the idle delay. The separate Aperture icon opens the application menu.

Live Activities, Wi-Fi, Battery and Control Center are excluded from hiding. Behavior depends on how macOS registers each icon and the available space. The feature does not universally reorder other applications’ icons.

## Appearance, fit and motion

Select **Black**, **Clear**, **Glass**, or **Half Glass** for the expanded island. In **Settings → General → Tuning**, adjust width/height by up to two display pixels in either direction. **Fit** is zero. The red preview follows the adjustment.

Hover delay, spring response, damping and optional haptics are configurable. Compatible trackpads provide the haptic feedback. Visibility options control full-screen apps, gaming and Mission Control. macOS Reduce Motion is respected by supported transitions.

## Permissions and data

Enable access for the features you choose. The app reports connection or permission problems in the corresponding Settings page.

| Feature | Access or data used |
| --- | --- |
| Music and Spotify | Automation for supported metadata and playback actions. |
| Browser controls / exposed Music queue | The Device Control and Data Access permission requested by the app, reading exposed controls and metadata. |
| Live waveform | System-output audio, analyzed in memory without saving an audio recording. |
| Calendar | Connected calendars for events and reminders. |
| Bluetooth | Device names/types for connection information. |
| Menu bar and keyboard controls | The macOS access requested by the selected control options. |
| Weather / time to leave | Selected city coordinates for Open-Meteo; mapped event locations for Apple Maps. |
| Up Next catalogue artwork | Song/artist metadata sent to Apple’s catalogue search, with matching album editions and artwork downloads. |
| Updates | GitHub release metadata when you use Check for Updates. |

Phone-call controls remain experimental and still need real incoming/outgoing validation. They are not presented as a verified release feature in this guide.

[Back to the visual feature guide](../README.md)
