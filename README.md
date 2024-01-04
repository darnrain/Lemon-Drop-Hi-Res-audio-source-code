## Lemon Drop Hi-Res audio source code

### Welcome to the future of music...
### The Lgv20 was first with the Android Nougat operating system.
### Now it's the first running in True Native Mode.
### With all 4 DACs enabled.
### A total of 98,304  channels in true stereo.

Lemon Drop Hi-Res development status: Active.<br>
latest release: v148.3<br>

Audio souce code for Lemon Drop Hi-Res<br>
Enable System wide QuadDAC support v8.2 aka build.prop audio tweaks.<br>
They both go hand and hand to increase the audio quality of the QuadDAC to the maximum.<br>

### This next part is how I found the True Native Mode code.
If your curious on how I found the True Native Mode code, I will show you. Someone left about 0.5% of the code in the original mixer_paths_tasha.xml file for the Lgv20. Go to line number 278 through 287 you will see the 0.5% of the True Native Mode code that I found. As you can see INI1, INI2, INI7, INI8, LO1, LO2, LO3, LO4 lines of code are partly there, the absolute perfect base starting point for me, to create the True Native Mode code. The other 99.5% I made with my own hands, all by myself. With trial and error and logic and my advanced Linux computer skills, if the code does not exist, make it yourself. No external resource was utilized, to my knowledge there is no  external resource of this nature. Once I found out that this was the ultimate puzzle. I had to solve it, out of extreme curiosity. What would the QuadDAC sound like running in True Native Mode? If you need more proof, I will give you the link to the Lgv20 rom that has this 0.5% True Native Mode code. https://androidfilehost.com/?fid=1322778262904012823
### end of how I found the True Native Mode code.

When programing a QuadDAC you do not have visual gauges to view to see if you have done something wrong, its all done by the sound of the DAC. For example if you have increased the amount of channels way to high or messed up on your programing code, then the DACs volume will be decreased or the music will not sound like its full of life. The only way to accomplish that, is to lower the AVC volume. In other words it decreases the power to the DAC so you can program and tune the DAC. In v142.1 and higher the AVC volume is set to the maximum. I know with out a doute that the True Native Mode code is pristine, I had echo print out the numbers, then I cut and pasted 768 times. I used nano's macro feature to program True Native Mode.<br>

What is True Native Mode on the Saber ESS 9218 DAC?<br>
I created all 1572 lines of the True Native Mode code, with the help of echo and nano, there are 786 mixer paths for True Native Mode that places the QuadDAC into it's highest performance state. The very essence of True Native Mode it's self allows the DAC to have more than two channels, like one for left and one for right. I have the QuadDAC overclocked so we can have more than 3072 channels. There are 768 channels going to each DAC, 768 X 64 = 49152 then divide 49152 by 2 = 24576 for each DAC for a total of 98304 channels. We can only hear up to 20kHz however the more channels there are the better the audio sounds to us, it's like SD video vs HD video.<br>

 From my understanding, this True Native Mode code will work on any Android phone that has a Saber ESS DAC, maybe even other brands of DACs. That is why I uploaded to GitHub so devs can add this code to there rom. all files are located in /system/vendor/etc/<br>
 
It is my understanding that the two files responsible for making this all happen are, audio_platform_info.xml and mixer_paths_tasha.xml. I disconnected the QuadDAC from the Android mixer in audio_platform_info.xml and programed the QuadDAC for True Native Mode in the mixer_paths_tasha.xml. The QuadDAC also needs Enable System wide QuadDAC support v8.2 aka build.prop audio tweaks. All the other files were from my previous attempts to increase the audio quality of the Lgv20 without avail. I have been working on this project for a long time, I lost track.<br>

At the very least you need these 4 build.prop lines to increase the buffer size for the QuadDAC so it can run in True Native Mode.<br>
audio.offload.size.kb=4096<br>
audio.offload.buffer.size.kb=8192<br>
venter.audio.offload.size.kb=4096<br>
venter.audio.offload.buffer.size.kb=8192<br>
 
I programed the mixer_paths all by myself by trial, error and logic. No external reference, there is no reference in existence to my knowledge. I just wanted a Hi-Res music player, but didn't want to pay $2000 for one, so I programed my Lgv20 to be a Hi-Res music player. I knew it had the same Saber ESS 9128 DAC as a Hi-Res music player, so if programed like a Hi-Res music player it should sound the same, and it does, maybe even better!<br>

I remember when I first found the True Native Mode code, I was like ooh what's that.<br>

What is True Native Mode on a computer?<br>
"(1) The normal running mode of a computer, executing programs from its built-in instruction set. Contrast with emulation mode. See native language. (2) The highest performance state of a computer."<br>

I guess you could say I have a gift that allows me to think outside of the box. I was always seeing LO in the True Native Mode code. I was like what is LO??? Then it hit me it's the bass. I came up with MI and HI for mid-range and treble myself and it worked!!! Also I was always seeing RX everywhere I looked, I was like well if there is an RX there has to be a TX. I guess you could say it was trial and error and logic is how I accomplished all of this. The devs that programed the Saber ESS DAC chip are professionals, you need to think like how they think. They would not make it to complicated to program the QuadDAC. To me it was the ultimate puzzle that needed to be solved and I did solve it. It feels good.<br>

What do I need to set my Hi-Res music player at?<br>
You need to choose 24bit 44.1kHz as the source, that's how I programed the DAC, it takes 24bit 44.1kHz and upsamples the audio eight times to 32bit 352.8kHz. On wired headphones the output is 32bit 352.8kHz, all other devices the output is 44.1kHz 24bit or 16bit. If set to anything other than, 44.1kHz the audio does not get upsampled eight times or it does not multiply evenly into what the DAC is set at 352.8kHz. In other words, your not going to get the absolute best audio quality.<br>
 
A little backstory.<br>
They left about 0.5% of the True Native Mode code in the mixer_paths file, I put the other 99.5% of the True Native Mode together myself. Just think if they would have never left that small peace of code in the mixer_paths file this would have never had happened. All I can say is that must have been a mistake, the Lgv60 does not have that small piece of code, only the Lgv20 does. I bet this is the same True Native Mode code as a $2000 Hi-Res music player. Most likely they have a computer program that programs the QuadDAC for True Native Mode, me on the other hand, this True Native Mode code was all hand made by me. So in other words, the Lgv20 will sound like no other Hi-Res music player in the world. A computer program cannot replace the very essence, of what a human is able to accomplish when programing a QuadDAC.<br>
 
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
