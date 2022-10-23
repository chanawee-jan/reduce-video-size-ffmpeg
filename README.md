## Steps to reduce video size using ffmpeg (for Mac M1) ##

## 1) Install homebrew

Open your terminal and execute following command.
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

## 2) Install ffmpeg

Search "ffmpgeg" in https://brew.sh/ and copy the command or using this command

`brew install ffmpeg`

## 3) To reduce the video resolution of mp4 file to half, using the follwing line

`ffmpeg -i input.mp4 -vf "scale=iw/2:ih/2" output.mp4`

## 4) To convert .mov to .mp4, using the following line

`ffmpeg -i input.mov -vcodec copy -acodec copy output.mp4`
