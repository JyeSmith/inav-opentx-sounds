# inav-opentx-sounds

This sound pack is for some of the modes found in INAV (https://github.com/iNavFlight) and can be used with OpenTX (https://github.com/opentx).

Below is an index of each wav.  Feel free to open an issue/pull if you would like to request a new sound.

```
inav00 - armed
inav01 - disarmed
inav02 - acro flight mode selected
inav03 - angle flight mode selected
inav04 - manual flight mode selected
inav05 - starting servo auto trim
inav06 - starting autotune
inav07 - altitude hold on
inav08 - way point mission started
inav09 - returning to home
```

## How to make more sounds

Sounds were synthesized using https://text-to-speech-demo.ng.bluemix.net/ and ```American English (en-US): Allison```.  Use the below in ```Voice Transformation SSML```, press Speak to test and the download for the mp3.

```
<voice-transformation type="Custom" breathiness="90%">
text to be synthesized 
</voice-transformation>
```

Sounds are downloaded as mp3 and can be converted to wav using ffmpeg.

```
ffmpeg -i song.mp3 -acodec pcm_s16le -ar 8000 -ac 1 song.wav
```

Add the wav files to your SD cards ```SOUNDS/en``` directory.

For more info on how to create and add custom sounds check out Project Blue Falcon https://www.youtube.com/watch?v=RZ8XwYgo8kg.
