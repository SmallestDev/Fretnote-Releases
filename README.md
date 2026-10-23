# Fretnote

Releases of **Fretnote**, a guitar chord practice app for Windows 10/11. Drop in a music file (MP3, WAV, FLAC,
M4A, OGG) or photos/PDFs of a chord chart and Fretnote finds the chords, beats, bars, time signature and key, then
plays the song while showing the current chord, the next chords and how to finger them, in sync with the music.
Practice with A-B and bar loops, 0.5–1.5× speed without pitch change, count-in and metronome, pick an easier capo
position, transpose, and correct any chord the analysis got wrong. Korean user interface, dark and light themes.

## Download
Open the [latest release](../../releases/latest) and download `Fretnote-windows-<version>-setup.exe`.

## Updates
The app includes an automatic update system.

A few seconds after Fretnote starts it checks this repository for a new version. If there is one, it shows what
changed and asks you; nothing is downloaded until you choose **Install**. The installer is verified against the
app's signing key before it runs, and if anything fails the current version keeps working. Your songs, edits,
settings and analysis cache are kept. You can turn the check off in **Settings**.

`latest.json` and the `.sig` file are used by the automatic updater. You don't need to download them.

## Installation
1. Download `Fretnote-windows-<version>-setup.exe`
2. Run it. It installs for the current user (no administrator rights) to `%LOCALAPPDATA%\Fretnote` and adds a Start menu entry
3. Start **Fretnote** and drag a song or a chord chart photo onto the window

> Windows may show "Windows protected your PC" because the installer isn't code-signed. Choose **More info** → **Run anyway**.

> Fretnote uses Microsoft Edge WebView2, which is part of Windows 11 and current Windows 10. If it is missing, the installer downloads it.

## Notes
- All analysis runs on your PC. Fretnote doesn't upload music or images and has no account or telemetry. The only network access is the update check against this repository.
- Chord recognition is automatic and can be wrong, especially with rich chords (maj7, sus) and dense mixes. Every chord, time and the tempo can be edited, and the original analysis is kept.
- Chord charts with printed chord symbols are read with the OCR built into Windows. Staff notation without chord symbols is detected but not converted to chords.
- Songs, edits and settings are kept in `%LOCALAPPDATA%\com.smallestdev.fretnote`. Uninstalling keeps them unless you tick "delete app data".
- `.sha256` files contain the SHA-256 checksum of each download.

If you encounter a problem, please report it so it can be fixed in a future update.
