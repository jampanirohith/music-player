# Music Player with Karaoke-Styled Lyrics
A browser-based karaoke music player with timed lyrics, local music-library scanning, album artwork, and a glass-black / midnight-blue interface.

## Features
- **Local music library:** Add music folders or individual files, rescan folders, and search the library.
- **Audio playback:** Play/pause, previous/next track, seek, volume, shuffle, and repeat.
- **Timed lyrics:** Display `.lrc` lyrics with line timing and supported word-timed formats.
- **Library views:** Switch between list and cover-grid layouts, sort by title/artist/folder, and filter songs with lyrics.
- **Artwork and metadata:** Read supported embedded audio tags and locate matching cover images.
- **Playback display:** Current-track information, lyric timing adjustment, fullscreen controls, and keyboard shortcuts.
- **Dark glass theme:** Translucent black surfaces, midnight-blue buttons, and responsive layouts.

## Supported Files

### Audio
MP3, M4A, AAC, FLAC, WAV, OGG, OGA, OPUS, and WEBA. Actual playback depends on browser codec support.

### Lyrics
Use `.lrc` files. Place the lyrics file next to the audio file and give both the same base filename:

```text
My Song.mp3
My Song.lrc
```

Example of line-timed lyrics:
```text
[ti:My Song]
[ar:My Artist]
[00:12.00]First line of the song
[00:16.50]Second line of the song
```

Word-timed timestamps are also supported:
```text
[00:12.00]<00:12.00>Hello <00:12.40>there
```

Ordinary line-timed lyrics use estimated word timing, so highlighting may be less precise than with word-timed lyrics.

### Artwork
The app can use embedded cover art, a matching image filename, or a folder cover image. Supported extensions include JPG, JPEG, PNG, WEBP, GIF, and BMP.

## Run Locally
1. Download the HTML file or project files.
2. For the separate-CSS version, keep `index.html` and `styles.css` in the same folder.
3. Open `index.html` in a modern browser such as Chrome or Edge.
4. Select **Add folder** or **Add files** and grant browser permissions when prompted.

If folder selection is unavailable, try **Compatibility mode** or use **Add files**.

## Use the website at:
```text
https://jampanirohith.github.io/music-player/
```

## Privacy and Permissions

The app is designed to process selected songs, lyrics, and cover images locally in your browser. It does not need to upload your music to a server.
Folder access depends on browser support and explicit permission. If you clear browser site data or revoke permission, you may need to add your folders again. Audio playback varies by browser and codec.
The app loads web fonts from Google Fonts when an internet connection is available and uses fallback fonts when they cannot load.

## Keyboard Shortcuts

| Key | Action |
|---|---|
| `Space` | Play or pause |
| `Left` / `Right` | Seek backward or forward by 5 seconds |
| `N` / `P` | Next / previous song |
| `F` | Toggle fullscreen |
| `L` | Show or hide the library |
| `M` | Mute |
