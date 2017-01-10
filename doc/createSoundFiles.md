## Custom sounds on Thymio

### Cheklist
* Max 10 sound files
* Has to be `mono` & `8000 Hz` & saved as `Unsigned 8 bit PCM` & `wav`
* SD card must be `FAT32`

### Creating sound

This is copied from the [Official Thymio documentation](https://www.thymio.org/en:thymioapi) for a quick reference.

You can create sounds for Thymio using your computer. An efficient way to do so is to use the Audacity software, version 1.3, which exists for various operating systems. Here are the steps to create a sound compatible with the Thymio:

Once Audacity has started, change the project rate from 44100 Hz (default) to 8000 Hz. This setting is located at the bottom-left of Audacity's window.
Record your sound with the red record key in the top-left part of the window. You should see the cursor advancing and the wave changing. Stop with the stop button.
Your sound should be in mono (Tracks->Stereo to Mono)
Go to the File menu under Export…
Give a file name, for instance P0.wav for the first file to play using the sound.play native function.
Choose other uncompressed files as format format.
Under options, choose a WAV (Microsoft) header and as Encoding, choose Unsigned 8 bit PCM.
Make sure that no metadata values ares set.
Save or copy the file to the micro-SD card.
To do a quick test, you can save this file under the name S0.wav. Thymio will play it when it starts.

Here's an instructional video on how to do the above.

Here is an A4 paper cheat sheet on how to do the above. (in french only)