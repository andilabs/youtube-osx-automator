# youtube-osx-automator
Download youtube videos as audio straight into apple Music.app


Needed homebrew packages:

install [yt-dlp](https://github.com/yt-dlp/yt-dlp)

```
sudo curl -L https://github.com/yt-dlp/yt-dlp/releases/latest/download/yt-dlp -o /usr/local/bin/yt-dlp
sudo chmod a+rx /usr/local/bin/yt-dlp  # Make executable
sudo yt-dlp -U
```


ffmpeg:

```
brew install ffmpeg
```


check command works:

```
yt-dlp --embed-metadata --downloader ffmpeg -P '/Users/andi/Music/Music/Media.localized/Automatically Add to Music.localized' -f 'bestaudio[ext=m4a]' https://www.youtube.com/watch?v=2Q_ZzBGPdqE
```

as result you should get song from this video https://www.youtube.com/watch?v=2Q_ZzBGPdqE inside Music.app  Recently added

