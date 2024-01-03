## Lemon Drop Hi-Res audio source code

### Welcome to the future of music...
### The Lgv20 was first with the Android Nougat operating system.
### Now it's the first running in True Native Mode.
### With all 4 DACs enabled.
### A total of 98,304  channels in true stereo.

Lemon Drop Hi-Res development status: Active.<br>
latest release: v145.1<br>

Audio souce code for Lemon Drop Hi-Res<br>
Enable System wide QuadDAC support v8.2 aka build.prop audio tweaks.<br>
They both go hand and hand to increase the audio quality of the QuadDAC to the maximum.<br>

The diff directory I uploaded the original then the modded v122.1, that way you can look at the commits from gound zero.<br>

What is True Native Mode?<br>
I created all 1572 lines of the True Native Mode code, with the help of echo and nano, there are 786 mixer paths for True Native Mode that places the QuadDAC into it's highest performance state. True Native Mode it's self allows the DAC to have more that one channel, like one for left and one for right. I have the QuadDAC over clocked so we can have more that 768 channels. There are 768 channels going to each DAC, 768 X 64 = 49152 then divide 49152 by 2 = 24576 for each DAC for a total of 98304 channels. We can only hear up to 20kHz however the more channels there are the better the audio sounds to us, it's like SD video vs HD video.<br>
 
I programed the mixer_paths all by myself by trial and error. No external reference, there is no reference in existence to my knowledge. I just wanted a Hi-Res music player, but didn't want to pay $2000 for one, so I programed my Lgv20 to be a Hi-Res music player. I knew it had the same Saber ESS 9128 DAC as a Hi-Res music player, so if programed like a Hi-Res music player it should sound the same, and it does, maybe even better!<br>

They left about 0.5% of the True Native Mode code in the mixer_paths file, I put the other 99.5% of the True Native Mode together myself. Just think if they would have never left that small piece of code in the mixer_paths file this would have never had happened. All I can say is that must have been a mistake, the Lgv60 does not have that small piece of code, only the Lgv20 does. I bet this is the same True Native Mode code as a $2000 Hi-Res music player. Most likely they have a computer program that programs the QuadDAC for True Native Mode, me on the other hand, this True Native Mode code was all hand made by me. So in other words, the Lgv20 will sound like no other Hi-Res music player in the world. A computer program cannot replace the very essence, of what a human is able to accomplish when programing a QuadDAC.<br>

My hope is to have people add this code to other Android roms, so everyone can experience what the future of music sounds like...<br>

Lemon Drop Hi-Res True Native Mode Stock Oreo Rom for the H910 & most Lgv20 phones.<br>
https://xdaforums.com/t/lemon-drop-hi-res-true-native-mode-stock-oreo-rom-for-the-h910-most-lgv20-phones.4432865/

MIT License<br>

Copyright (c) 2023 darnrain<br>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:<br>

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.<br>

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.<br>
