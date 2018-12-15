# OperaFixUbuntu18
Fix for opera html5 video in Ubuntu18

```
# install chrome and extra ffmpeg for chrome
sudo apt install chromium-codecs-ffmpeg-extra chromium-browser

# backup old ffmpeg in opera folder
sudo mv /usr/lib/x86_64-linux-gnu/opera/libffmpeg.so /usr/lib/x86_64-linux-gnu/opera/libffmpeg.BACKUP

# copy over from chrome
sudo cp /usr/lib/chromium-browser/libffmpeg.so /usr/lib/x86_64-linux-gnu/opera/.

# change to executable write
sudo chmod +x /usr/lib/x86_64-linux-gnu/opera/libffmpeg.so
```
