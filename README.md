# ymusic — Desktop Y0uTu6e Music Player

A lightweight GTK4 desktop player for YouTube Music using `mpv` + `yt-dlp`. Search tracks, get recommendations, and save your likes — all from your desktop.

## Features

- Search YouTube tracks and play audio only
- Recommendations based on current track
- Like/unlike tracks (saved locally)
- Play All / Shuffle liked tracks
- Seek, volume, loop controls
- Keyboard shortcuts

## Dependencies

- Python 3
- GTK4 (`libgtk-4-dev` / `gtk4` / `pygobject`)
- `mpv`
- `yt-dlp`
- `deno` (for JavaScript runtime, required by yt-dlp for YouTube extraction)

## Install

```bash
# Clone the repo
git clone https://github.com/yourusername/ytmusic.git
cd ytmusic

# Make executable
chmod +x ymusic

# Run
./ymusic
```

Or move it to your PATH:

```bash
cp ymusic ~/.local/bin/
```

## Usage

| Action             | Description                          |
|--------------------|--------------------------------------|
| Search bar + Enter | Search YouTube tracks                |
| Ctrl+F             | Focus search bar                     |
| Ctrl+L             | Show liked songs                     |
| ▶ Play             | Start a track                        |
| ♡ / ♥             | Like / Unlike a track                |
| ⏹ Stop             | Stop playback                        |
| ▶ / ⏸             | Play / Pause                         |
| ⏮ / ⏭             | Prev / Next (in queue)               |
| 🔂                 | Toggle loop one                      |
| 🔀 Shuffle         | Shuffle and play liked songs         |
| ▶ Play All         | Play all liked songs in order        |

## Storage

- Liked tracks: `~/.cache/ymusic/liked.json`
- Cache files: `~/.cache/ymusic/`

## License

MIT
