# go-vod

Extremely minimal on-demand video transcoding server in go.

## Usage

You need go and ffmpeg/ffprobe installed

```bash
CGO_ENABLED=0 go build -ldflags="-s -w"
./go-vod
```

The server exposes all files as HLS streams, at the URL
```
http://localhost:47788/player-id/path/to/file/index.m3u8
```