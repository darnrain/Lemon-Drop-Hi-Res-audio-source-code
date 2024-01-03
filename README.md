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

What is True Native Mode on the Saber ESS 9218 DAC?<br>
I created all 1572 lines of the True Native Mode code, with the help of echo and nano, there are 786 mixer paths for True Native Mode that places the QuadDAC into it's highest performance state. The very essence of True Native Mode it's self allows the DAC to have more than two channels, like one for left and one for right. I have the QuadDAC over clocked so we can have more than 3072 channels. There are 768 channels going to each DAC, 768 X 64 = 49152 then divide 49152 by 2 = 24576 for each DAC for a total of 98304 channels. We can only hear up to 20kHz however the more channels there are the better the audio sounds to us, it's like SD video vs HD video.<br>

From my understanding, this True Native Mode code will work on any Android phone that has a Saber ESS DAC, maybe even other brands of DACs. That is why I uploaded to GitHub so devs can add this code to there rom.<br>

It is my understanding that the two files responsible for making this all happen are, audio_platform_info.xml and mixer_paths_tasha.xml. I disconnected the QuadDAC from the Android mixer in audio_platform_info.xml and programed the QuadDAC for True Native Mode in the mixer_paths_tasha.xml. All the other files were from my previous attempts to increase the audio quality of the Lgv20.

I programed the mixer_paths all by myself by trial, error and logic. No external reference, there is no reference in existence to my knowledge. I just wanted a Hi-Res music player, but didn't want to pay $2000 for one, so I programed my Lgv20 to be a Hi-Res music player. I knew it had the same Saber ESS 9128 DAC as a Hi-Res music player, so if programed like a Hi-Res music player it should sound the same, and it does, maybe even better!<br>

I remember when I first found the True Native Mode code, I was like ooh what's that.<br>

What is True Native Mode on a computer?<br>
"(1) The normal running mode of a computer, executing programs from its built-in instruction set. Contrast with emulation mode. See native language. (2) The highest performance state of a computer."<br>

I guess you could say I have a gift that allows me to think outside of the box. I was always seeing LO in the True Native Mode code. I was like what is LO??? Then it hit me it's the bass. I came up with MI and HI for mid-range and treble myself and it worked!!! Also I was always seeing RX everywhere I looked, I was like well if there is an RX there has to be a TX. I guess you could say it was trial and error and logic is how I accomplished all of this. The devs that programed the Saber ESS DAC chip are professionals, you need to think like how they think. They would not make it to complicated to program the QuadDAC. To me it was the ultimate puzzle that needed to be solved and I did solve it. It feels good.<br>
 
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
