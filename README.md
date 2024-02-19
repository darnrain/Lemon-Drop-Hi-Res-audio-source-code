![294729981-1fd80758-cdef-4be1-afb5-1d6666d383a0](https://github.com/darnrain/Lemon-Drop-Hi-Res-audio-source-code/assets/60840489/c7f73ce2-8e2e-4c9c-955c-38dced1bd54c)
# Welcome to the future of music... 
### Lemon Drop Hi-Res audio source code
Welcome to the worlds best & first 24/32bit QuadDAC in True Stereo!<br>
The 16bit side is set at: 64bit, 176.4kHz with 6411 channels and upsampled 4X from 16bit, 44.1Khz<br>
The 24bit side is set at: 384bit, 705.6kHz with 24576 channels and upsampled 16X from 16bit, 44.1kHz<br>
24bit QuadDAC 24 X 4 = 96<br>
Running in True Native Mode.<br>
With all 4 DACs running independently.<br>
DAC 0 = low-range - volume 51 - 96bit - 176.4kHz - 6144 channels.<br>
DAC 1 = mid-range - volume 53 - 96bit - 176.4kHz - 6144 channels.<br>
DAC 2 = high-range - volume 55 - 96bit - 176.4kHz - 6144 channels.<br>
DAC 3 = offload - volume 57 - 96bit - 176.4kHz - 6144 channels.<br>

Please listen at a safe volume level.<br>

Latest version: v218.1<br>

### Introduction
I’m not going to beat around the bush. I reinvented stereo. I also invented the worlds first 24/32bit QuadDAC. I also invented Hardware Offloaded Audio Processing on Android. In other words all audio including bluetooth is routed through the QuadDAC. Android has no say, when it has to do with the audio. This also means that the QuadDAC must stay enabled at all times. This was the only way, I was able to get around the audio limitations set in place by Android. In other words, checkmate.<br>

"You take the blue pill—the story ends, you wake up in your bed and believe whatever you want to believe. You take the red pill—you stay in Wonderland and I show you how deep the rabbit-hole goes."<br>
— Morpheus<br>

"For every action there is an equal and opposite reaction."<br>
— Sir Isaac Newton<br>

"We live in a crooked world, with crooked people, with crooked music."<br>
— darnrain<br>

“Once you eliminate the impossible, whatever remains, no matter how improbable, must be the truth”<br>
— Sir Arthur Conan Doyle<br>

“I have not failed. I've just found 10,000 ways that won't work.”<br>
— Thomas Edison<br>

### What is True Native Mode on a computer?
"(1) The normal running mode of a computer, executing programs from its built-in instruction set. Contrast with emulation mode. See native language. (2) The highest performance state of a computer."<br>

### What is True Native Mode on the Saber ESS 9218 DAC?<br>
I created all 4632 lines of v3.0 True Native Mode code myself, with the help of sed, awk, echo, nano and l3afpad. True Native Mode it's self places the QuadDAC into it's highest performance state. Not only does it place the QuadDAC in it's highest performance state, you also have root access to program the QuadDAC, anything you can imagine. This is what I imagined: The worlds first 24/32bit QuadDAC in True Stereo! The very essence of True Native Mode it's self allows the QuadDAC, to have more than two channels for stereo. The more channels, the better the audio sounds to us.<br>

### How did you find this True Native Mode code?
If your curious on how I found the True Native Mode code, I will show you. Someone left about 0.5% of the code in the original mixer_paths_tasha.xml file for the Lgv20. Go to line number 278 through 287 you will see the 0.5% of the True Native Mode code that I found. As you can see, INI1 HPHL, INI2 HPHR, INI7 SPKRL, INI8 SPKRR, INI3 LO1, INI4 LO2, INI5 LO3, INI6 LO4, lines of code are partially there, the absolute perfect base starting point for me, to recreate the True Native Mode code. LO1 even started with INI3 that gave me my first clue. The other 99.5% I made with my own hands, all by myself. With trial and error and logic and my advanced Linux computer skills, if the code does not exist, make it yourself. No external resource was utilized, to my knowledge a resource of this nature absolutely does not exist. If you want to confirm that this original mixer_paths_tasha.xml is authentic, I will give you the link to the Lgv20 rom that has this 0.5% True Native Mode code.<br> https://androidfilehost.com/?fid=1322778262904012823

Update: I found the missing piece to the puzzle. Look in the original mixer_paths_tasha.xml. Line number: 549 - 552. That's so odd, it's almost like someone left bread crumbs deliberately for me to follow.<br>

### My music does not sound Overpowered sometimes?
Can be due to the following:<br>
1. The QuadDAC was not able to acquire the precise Ohm rating of your headphones, to fix unplug your headphones and plug them back in.<br>
2. The phone is in low power mode.<br>
3. Your battery is to low, it is undetermined on how much battery power we must have. I would say at least over 15%.<br>

### How did you program and tune the QuadDAC?
When programing a QuadDAC you do not have visual gauges to view to see if you have done something wrong, its all done by the sound of the DAC. For example if you have increased the amount of channels way to high or messed up on your programing code, then the DACs volume will be decreased or the music will not sound like its full of life. To answer the question, I did it all by ear.

I was always seeing LO in the True Native Mode code. I was like what is LO??? Then it hit me it's low-range. I came up with MI and HI for mid-range and high-range myself and it worked!!! Also I was always seeing RX everywhere I looked, I was like well if there is an RX there has to be a TX. It was just dumb luck, that the TX must be on top of RX. I guess you could say it was trial, error, logic and my advanced Linux computer skills, is how I programed the Saber ESS 9218 DAC. The devs that programed the Saber ESS DAC chip are professionals, you need to think like how they think. They would not make it to complicated to program the QuadDAC. For me it was the worlds ultimate puzzle.<br>

### What's the audio offset to the worlds audio?
Keep in mind this may not be the correct offset, this is what sounded best to me.<br>

L = -14.4<br>
R = -28.4<br>

### Will this True Native Mode code work on other Android phones other than the Lgv20?
I can't say for absolutely certain, I can say for certain that the True Native Mode code runs excellent, on both of my Lgv20's, my main phone DeGoogled and the spare one with Google intact both running Stock Oreo ezV2020 v1.0 Kernel.  Who knows this True Native Mode code may work universally across all QuadDACs on all Android phones. It's up to you guys to beta test this code, my job is all done, I just had to recreate the True Native Mode code and make it work. The LG V series of phones, will have the best chance of this True Native Mode code working. Also keep in mind that I officially got True Native Mode working in v169.1, on 01-17-24 phones manufactured after that date may have True Native Mode disabled on the QuadDAC chip.<br>

### I want to add this True Native Mode code, to my Android phone?
My theory is that the two files responsible for making this all happen are, audio_platform_info.xml and mixer_paths_tasha.xml. All the other files are associated with the Android mixer and are the left over reminisce of my previous attempts of trying to increase the audio quality on the Lgv20 without avail. The initial mixer settings is the most important part of the QuadDAC. If there are duplicates or errors or mistakes in that location. Then it will effect the audio quality of the QuadDAC and or the QuadDAC will simply not function. You will know when you have messed up, your phone will not boot and or there will be no sound. There is over 6,000 lines of code in that location. If you are attempting to add my code to your mixer_paths file. Just remember that this is a puzzle, and 95% of the peaces were missing. I not only had to make the 95% of the missing code and program the QuadDAC. I also had to fight with the original mixer_paths file, it was FUBAR. Who ever programed the Lgv20's original mixer_paths.xml file, had absolutely no clue what they where doing. This was very challenging for me, and fun. You will also need to make the missing peaces of your unique initial mixer settings. You need to work in the initial mixer settings, as well as adding my code to your mixer_paths file. I already programed the QuadDAC, you just need to make sure the initial mixer settings are the same as your phone. Your welcome to delete the initial mixer settings of the Lgv20, some settings are going to be the same like the volume settings. It's going to take time, it has taken me over a year.<br>

The QuadDAC also needs Enable System wide QuadDAC support v8.2 aka build.prop audio tweaks. The QuadDAC needs exactly 4MB cache size. This also will enable Hardware Offloaded Audio Processing. In other words all audio including bluetooth is routed through the QuadDAC. Android has no say, when it has to do with the audio. This also means that the QuadDAC must stay enabled at all times. This was the only way, I was able to get around the audio limitations set in place by Android. In other words, checkmate.<br>

When programing the mixer_paths file, I only use the tab key not the spacebar, it's just a pet peeve. ;)<br>

I cant program with how disorganized the original mixer_paths file is. This is how I tabbed all lines and fixed it. I use arch linux.<br>

Example:
<pre>
cat your_mixer_paths_file.xml | sed 's/^[ \t]*//' > new_mixer_paths_file.xml
</pre>

sed commands:<br>
Move all lines to the left:<br>
<pre>
sed 's/^[ \t]*//'
</pre>
Tab all lines:<br>
<pre>
 sed 's/^/\t/'
</pre>

This is how I debugged the code. I copied a section, pasted into a file test.txt then removed all the lines that have RX. Then I looked over test1.txt there should be groups of 4 or 3 and so on. If not then I knew I messed up. I did the same thing with RX.<br>
<pre>
 cat test.txt | grep TX > test1.txt
</pre>

The mixer_paths.xml file must have zero duplicates, or your phone will not boot. The initial mixer settings is the most important part, there should be zero duplicates, zero mistakes, zero errors. Copy a section, paste it into a file test.txt. This command will print all duplicates including all the spaces. A little tip, if you stdout into a file. Just scroll down all the spaces are at the top. lol
<pre>
sort test.txt | uniq -D
</pre>

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
