# OpenAI Whisper

## Python 3.8.6

## Guide on how to use OpenAI's Whisper speech recognition model with Python.

## Installation

1. Download FFmpeg 'ffmpeg-master-latest-win64-gpl.zip' from https://github.com/BtbN/FFmpeg-Builds/releases
2. Unzip the downloaded file and move the its content to a directory of your choice (e.g., `C:\path\bin`).
3. Add the directory where `ffmpeg.exe` is located to the `User variables for User` `Path` environment variable. 


Check in CMD of IDE terminal 'ffmpeg -version':
```
...
  libavutil      58.  6.100 / 58.  6.100
  libavcodec     60.  9.100 / 60.  9.100
  libavformat    60.  4.101 / 60.  4.101
  libavdevice    60.  2.100 / 60.  2.100
  libavfilter     9.  5.100 /  9.  5.100
  libswscale      7.  2.100 /  7.  2.100
  libswresample   4. 11.100 /  4. 11.100
  libpostproc    57.  2.100 / 57.  2.100
...
```

## Usage

1. Install the `ffmpeg-python` package by running `pip install ffmpeg-python`.
2. Load the Whisper model and transcribe an audio file by running the following code:

``` 
import whisper

model = whisper.load_model("base")
result = model.transcribe("audio.mp3")
print(result["text"])
```

## References

1. OpenAI Whisper: https://github.com/openai/whisper
2. Hub for installing OpenAI Whisper: https://hub.tcno.co/ai/whisper/install/
3. How to run OpenAI's Whisper speech recognition model: https://www.assemblyai.com/blog/how-to-run-openais-whisper-speech-recognition-model/
4. Download FFmpeg: https://ffmpeg.org/download.html#build-windows
 
