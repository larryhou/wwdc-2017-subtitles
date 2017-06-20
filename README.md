# wwdc-2017-subtitles
Subtitles for session videos in WWDC 2017

You can convert `*.webvtt` to `*.srt`(or some other format) with `ffmpeg`

```bash
find . -iname '*.webvtt' | while read vtt
do
	echo "ffmpeg -i ${vtt} $(echo ${vtt}| sed 's/\.webvtt$/\.srt/') -y" | xargs -I{} bash -c "{}"
done
```
TODO
209
214
218
219
225
237
241
242
243
245
402
412
414
416
509
511
512
514
606
610
706
712
715
716
802
811
813
814
816
