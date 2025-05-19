 # 51cg1-download

Pure browser-only webpage to download videos from 51cg1. 

No server, no downloads/app required, one single HTML; everything runs on your browser's JavaScript!

## How it works

51cg1 uses [Dplayer](https://github.com/DIYgod/DPlayer) to serve videos via m3u8. Its manifest contains a list of fragmented, encrypted .ts video files.

The work is simple:
1) Extract encryption key and IV
2) Download and decrypt each fragment
3) Merge fragments together
4) Video is ready to be downloaded

## TODOs

In order of priority (from highest to lowest):

- ~Loading/progress bar~
- Thumbnails for each video
- Support downloading as .mp4

## License

MIT

License may change if I eventually decide to use ffmpeg for .ts to .mp4 conversion.
