![294729981-1fd80758-cdef-4be1-afb5-1d6666d383a0](https://github.com/darnrain/Lemon-Drop-Hi-Res-audio-source-code/assets/60840489/c7f73ce2-8e2e-4c9c-955c-38dced1bd54c)
## Lemon Drop Hi-Res audio source code

Welcome to the future of music...<br>
The Lgv20 was first with the Android Nougat operating system.<br>
Now it's the first running in True Native Mode.<br>
With all 4 DACs enabled.<br>
A total of 98,304  channels in true stereo.<br>

Warning!!!<br>
Lemon Drop Hi-Res is more than capable of causing permanent damage to your hearing.<br>
Please listen at a safe volume level.<br>

Lemon Drop Hi-Res development status: Active.<br>
latest release: v163.1<br>

### How did you find this True Native Mode code?
If your curious on how I found the True Native Mode code, I will show you. Someone left about 0.5% of the code in the original mixer_paths_tasha.xml file for the Lgv20. Go to line number 278 through 287 you will see the 0.5% of the True Native Mode code that I found. As you can see, INI1 HPHL, INI2 HPHR, INI7 SPKRL, INI8 SPKRR, INI3 LO1, INI4 LO2, INI5 LO3, INI6 LO4, lines of code are partially there, the absolute perfect base starting point for me, to create the True Native Mode code. LO1 even started with INI3 that gave me a clue. The other 99.5% I made with my own hands, all by myself. With trial and error and logic and my advanced Linux computer skills, if the code does not exist, make it yourself. No external resource was utilized, to my knowledge there is no  external resource of this nature. If you want to confirm that this original mixer_paths_tasha.xml is authentic, I will give you the link to the Lgv20 rom that has this 0.5% True Native Mode code.<br> https://androidfilehost.com/?fid=1322778262904012823

### How did you transform the Lgv20 into A Professional High Resolution Audio Player?
For those that don't know, the mixer_paths_tasha.xml file is how you program the, Saber ESS 9128 DAC. I'm not going to beat around the bush, there is no easy way to say it, in my professional opinion the original mixer_paths_tasha.xml file is totally fu#$%d up. I have always known without an absolute doubt in my mind, that someone deliberately sabotaged the original mixer_paths_tasha.xml file, or they just suck really bad at programing. It's hard for me to believe that someone could suck that bad at programing, that's programing the original mixer_paths_tasha.xml file for every single Lgv20 phone ever made. I was always asking myself, now what did they sabotage this time? I went in there with a mind set, someone sabotaged the original mixer_paths_tasha.xml file, and I need to fix it. It was like a treasure hunt to me, I had some of the most fun in my entire life, trying to locate and fix everything that they sabotaged. So with trial, error, logic, and my advanced Linux computer skills and the knowledge of knowing that someone deliberately sabotaged the original mixer_paths_tasha.xml file, is how I have successfully transformed my Lgv20 into a Professional High Resolution Audio Player.<br>

### What is True Native Mode on a computer?
"(1) The normal running mode of a computer, executing programs from its built-in instruction set. Contrast with emulation mode. See native language. (2) The highest performance state of a computer."<br>

### What is True Native Mode on the Saber ESS 9218 DAC?<br>
I created all 1568 lines of the True Native Mode code myself, with the help of echo and nano, there are 786 mixer paths for True Native Mode that places the QuadDAC into it's highest performance state. The very essence of True Native Mode it's self allows the DAC to have more than two channels, like one for left and one for right. I have the QuadDAC overclocked so we can have more than 3072 channels. There are 768 channels going to each DAC, 768 X 64 = 49152 then divide 49152 by 2 = 24576 for each DAC for a total of 98304 channels. We can only hear up to 20kHz however the more channels there are the better the audio sounds to us, it's like SD video vs HD video.<br>

### How did you program and tune the QuadDAC?
When programing a QuadDAC you do not have visual gauges to view to see if you have done something wrong, its all done by the sound of the DAC. For example if you have increased the amount of channels way to high or messed up on your programing code, then the DACs volume will be decreased or the music will not sound like its full of life. The only way to accomplish that, is to lower the AVC volume. In other words it decreases the power to the DAC so you can program and tune the DAC. In v142.1 and higher the AVC volume is set to the maximum. I know with out a doute that the True Native Mode code is pristine, I had echo print out the numbers, then I cut and pasted 768 times. I used nano's macro feature to program True Native Mode.<br>

I guess you could say I have a gift that allows me to think outside of the box. I was always seeing LO in the True Native Mode code. I was like what is LO??? Then it hit me it's the bass. I came up with MI and HI for mid-range and treble myself and it worked!!! Also I was always seeing RX everywhere I looked, I was like well if there is an RX there has to be a TX. I guess you could say it was trial, error, logic and my advanced Linux computer skills, is how I programed the Saber ESS 9218 DAC. The devs that programed the Saber ESS DAC chip are professionals, you need to think like how they think. They would not make it to complicated to program the QuadDAC. To me it was the ultimate puzzle that needed to be solved and I did solve it. It feels good.<br>

### I want to add this True Native Mode code, to my Android phone?
It is my understanding that the two files responsible for making this all happen are, audio_platform_info.xml and mixer_paths_tasha.xml. This is only a theory, I am 98% positive, that you only need to mod those two files. Duplicate all the changes I made leaving intact your unique settings. I made notes in both files, to help you along the way. This is not for the novice computer user. The mixer_paths file must have zero typos, zero mistakes, zero errors. The QuadDAC also needs Enable System wide QuadDAC support v8.2 aka build.prop audio tweaks.<br>

Update: You should hold off on doing this, tell v164.1. I marked everthing I modded, yeah I was not thinking ahead. There are a few lines of code that are unique to the Lgv20 only and should not be duplicated. I am going to fix my notes in the mixer_paths file.<br>

I never even thought about making a guide on how to do this. I don't even know were to start. This was such a HUGE undertaking. I will do my best to give you a head start. I recommend using linux, I know you can copy 5558 lines of code to the clip board in linux. Let's talk about the mixer_paths_tasha.xml file. Your file may have a different file name, that's fine. First thing you want to do is copy from line number 29 to line number 5558 and paste in your mixer_paths file at the very top, well under the copyright notice. Then you can get to work deleting and adding all the changes I made to the mixer_paths file. Everything I deleted of importance is included in the 5558 lines of code I programed, including all the functions. I did my best to make the code extremely organised. Everything must be duplicated exactly, as I have programed the mixer_paths file. However the lines of code I deleted, you can actually delete your lines of code. The only thing I can think of is that the name of your DACs volume control may be diffrent, line number 1733 to 1736. Search for volume control to view volume settings. The initial mixer settings must start with a 0 or ZERO to program the DAC. It lets the DAC know what settings can be changed. If not then they are hard coded in the DACs settings and can not be changed such as the individual volume settings. If there is a typo or an error in the mixer_paths file then your phone will not boot, or it will boot and you will have no sound. I did add some important notes in the mixer_paths file. There can not be any duplicates, you must delete everything that I deleted zero duplicates, or phone will not boot. This is going to take a lot of time and patience. So what it boils down to, is you want to take all the changes that I made from the modded mixer_paths file and add them to your mixer_paths file, leaving intact your unique mixer_paths file settings. The Lgv20 has an FM radio, most phones to my knowledge do not have an FM radio. Oh and I recommend starting at v163.1 or higher. I was still working out all the bugs in the past versions. That version as far as I know, is absolutely flawless.<br>

Make sure there are only one of each <mixer\> and </mixer\> top and bottom. They can not be tabbed.<br>

When programing the mixer_paths file, I only use the tab key not the spacebar, it's just a pet peeve. ;)<br>

I cant program with how disorganized the original mixer_paths file is. This is how I tabbed all lines and fixed it. I use arch linux.<br>

Example:
<pre>
cat your_mixer_paths_file.xml | sed 's/^[ \t]*//' > new_mixer_paths_file.xml
</pre>

sed commands:<br>
Move all lines to the left.<br>
<pre>
sed 's/^[ \t]*//'
</pre>
Tab all lines.<br>
<pre>
 sed 's/^/\t/'
</pre>
### Will this True Native Mode code work on other Android phones other than the Lgv20?
Short answer, yes. As long as your phone has a Saber ESS QuadDAC.

### What do I need to set my Hi-Res music player at?
You need to choose 24bit 44.1kHz as the source, that's how I programed the DAC, it takes a 44.1kHz audio signal and upsamples the audio eight times to 32bit 352.8kHz. On wired headphones the output is 32bit 352.8kHz, all other devices the output is 44.1kHz 24bit or 16bit. If set to anything other than, 44.1kHz the audio does not get upsampled eight times or it does not multiply evenly into 352.8kHz. In other words, your not going to get the absolute best audio quality.<br>
 
### A little backstory.
I remember when I first found the True Native Mode code, I was like ooh what's that. Then I looked up online what True Native Mode was, the highest performance state of a computer, I was like cool. They left about 0.5% of the True Native Mode code in the original mixer_paths_tasha.xml file, I put the other 99.5% of the True Native Mode code together myself. Just think if they would have never left that small peace of code in the original mixer_paths_tasha.xml file this would have never had happened. Even more strange is that the 0.5% of the code I found, had the headphone side and the DAC side even the mixer paths, in other words everything was there to recreate the True Native Mode code. Almost like someone left it there deliberately? It's like if someone gave you the secret formula to make GOLD, wouldn't the first thing on your mind be, let's make some GOLD!!!

Most likely they have a computer program that programs the QuadDAC for True Native Mode, me on the other hand, this True Native Mode code was all hand made by me. So in other words, the Lgv20 will sound like no other Hi-Res music player in the world. A computer program cannot replace the very essence, of what a human is able to accomplish when programing a QuadDAC.<br>

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
