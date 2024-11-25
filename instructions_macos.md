First convert the audio file to .wav format


<code>ffmpeg -i input.mp3 -ar 16000 -ac 1 -c:a pcm_s16le output.wav</code>

Make sure to include the whole path for both the input and output file, for example, if you have your audio file in the downloads folder, you have to out this into the terminal.


<code>ffmpeg -i ./Downloads/myaudio.mp3 -ar 16000 -ac 1 -c:a pcm_s16le ./Downloads/myaudio.wav</code>


To run the transcription, consider this base line of code

<code>./main -m models/ggml-base.en.bin -f samples/jfk.wav</code>

but first, you have to go your directory where whispercpp is stored:

<code> </code>
```bash

```