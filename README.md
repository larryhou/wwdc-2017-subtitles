# wwdc-2017-subtitles
Subtitles for session videos in WWDC 2017

You can convert `*.webvtt` to `*.srt`(or some other format) with `ffmpeg`

```bash
find . -iname '*.webvtt' | while read vtt
do
	echo "ffmpeg -i ${vtt} $(echo ${vtt}| sed 's/\.webvtt$/\.srt/') -y" | xargs -I{} bash -c "{}"
done
```
