![294729981-1fd80758-cdef-4be1-afb5-1d6666d383a0](https://github.com/darnrain/Lemon-Drop-Hi-Res-audio-source-code/assets/60840489/c7f73ce2-8e2e-4c9c-955c-38dced1bd54c)
## Lemon Drop Hi-Res audio source code

### Welcome to the future of music...<br>
The worlds first 24bit QuadDAC.<br>
Set at: 384bit, 705.6kHz, 24576 channels.<br>
Running in True Native Mode.<br>
With all 4 DACs enabled.<br>
DAC 0 = low-range<br>
DAC 1 = mid-range<br>
DAC 2 = high-range<br>
DAC 3 = offload<br>

Please listen at a safe volume level.<br>

Lemon Drop Hi-Res development stage: Number three.<br>

1. You need to program the QuadDAC.<br>
2. You need to setup the QuadDAC.<br>
3. You need to check for errors or typos in your code.<br>
4. Finished.<br>

latest release: v192.1<br>

I recommend only using the latest version. I'm making enormous modifications to the operation of the QuadDAC. Lemon Drop Hi-Res is very much in the development stage.<br>

“I have not failed. I've just found 10,000 ways that won't work.”<br>
— Thomas Edison<br>

### What is True Native Mode on a computer?
"(1) The normal running mode of a computer, executing programs from its built-in instruction set. Contrast with emulation mode. See native language. (2) The highest performance state of a computer."<br>

### What is True Native Mode on the Saber ESS 9218 DAC?<br>
I created all 4632 lines of v3.0 True Native Mode code myself, with the help of sed, awk, echo, nano and l3afpad. True Native Mode it's self places the QuadDAC into it's highest performance state. Not only does it place the QuadDAC in it's highest performance state, you also have root access to program the QuadDAC, anything you can imagine. This is what I imagined: 384bit, 705.6kHz, 24576 channels. The very essence of True Native Mode it's self allows the QuadDAC, to have more than two channels for stereo. The more channels, the better the audio sounds to us.<br>

### How did you find this True Native Mode code?
If your curious on how I found the True Native Mode code, I will show you. Someone left about 0.5% of the code in the original mixer_paths_tasha.xml file for the Lgv20. Go to line number 278 through 287 you will see the 0.5% of the True Native Mode code that I found. As you can see, INI1 HPHL, INI2 HPHR, INI7 SPKRL, INI8 SPKRR, INI3 LO1, INI4 LO2, INI5 LO3, INI6 LO4, lines of code are partially there, the absolute perfect base starting point for me, to recreate the True Native Mode code. LO1 even started with INI3 that gave me my first clue. The other 99.5% I made with my own hands, all by myself. With trial and error and logic and my advanced Linux computer skills, if the code does not exist, make it yourself. No external resource was utilized, to my knowledge a resource of this nature absolutely does not exist. If you want to confirm that this original mixer_paths_tasha.xml is authentic, I will give you the link to the Lgv20 rom that has this 0.5% True Native Mode code.<br> https://androidfilehost.com/?fid=1322778262904012823

Update: I found the missing piece to the puzzle. Look in the original mixer_paths_tasha.xml. Line number: 549 - 552. That's so odd, it's almost like someone left bread crumbs deliberately for me to follow.<br>

### My music does not sound Overpowered sometimes?
Can be due to the following:<br>
1. The QuadDAC was not able to acquire the precise Ohm rating of your headphones, to fix unplug your headphones and plug them back in.<br>
2. The phone is in low power mode.<br>
3. Your battery is to low, it is undetermined on how much battery power we must have. I would say at least over 15%.<br>

### How did you program and tune the QuadDAC?
When programing a QuadDAC you do not have visual gauges to view to see if you have done something wrong, its all done by the sound of the DAC. For example if you have increased the amount of channels way to high or messed up on your programing code, then the DACs volume will be decreased or the music will not sound like its full of life. The only way to accomplish that, is to lower the AVC volume. In other words it decreases the power to the DAC so you can program and tune the DAC. In v142.1 and higher the AVC volume is set to the maximum. To answer the question, I used my 34 years of advanced computer skills and used, awk, sed, echo and nano to create the True Native Mode code.

I was always seeing LO in the True Native Mode code. I was like what is LO??? Then it hit me it's the bass. I came up with MI and HI for mid-range and treble myself and it worked!!! Also I was always seeing RX everywhere I looked, I was like well if there is an RX there has to be a TX. I guess you could say it was trial, error, logic and my advanced Linux computer skills, is how I programed the Saber ESS 9218 DAC. The devs that programed the Saber ESS DAC chip are professionals, you need to think like how they think. They would not make it to complicated to program the QuadDAC. For me it is the ultimate puzzle.<br>

### How did you calculate the numbers?<br>
I reprogrammed the QuadDAC, it’s now set at 384bit, 705.6kHz, 24576 channels. All the other versions I calculated the bit rate from the starting point of 16, this version I started at 24. Everything divides evenly into 24, 384 divided by 16 = 24, 705.6 divided by 16 = 44.1. That begs the question, why are Hi-Res music players still using 32bit? The world has moved on to 24bit audio. You know when kids try and fit a square into a circle, well the bit rates are exactly the same. You can not fit 24bit audio into a 32bit DAC, it’s just simply impossible. The only way to fit a square into a circle would be to trim the edges of the square and make it into a circle, before it will fit into the hole that is a circle. So what the DAC does, it makes it fit, it will trim off the edges of the square and make it into a perfect circle. Then it will fit into a 32bit DAC, so in other words the numbers must divide evenly into what the DAC is set at. The audio is actually cut, in other words the audio never reaches your ears. So 24bit audio is cut down to 16bit audio, 28.57% of the audio is just simply gone. Something else that will blow your mind, no one has ever heard what 24bit audio sounds like in the entire existence of 24bit audio, tell now that is. Welcome to the worlds first 24bit QuadDAC!<br>

How do I know this information, I have successfully programed a QuadDAC. Thanks to my 34 years of advanced computer experience. Need I say more?<br>

But the question in the back of my mind is why?<br>
1. They just never got around to reprogram a DAC to 24bit.<br>
2. It would cost to much money to produce a 24bit DAC chip.<br>
3. I am the first person to discover this, out of everyone in the entire world.<br>
4. Or the final scenario is, I just opened up Pandora's box. ;)<br>

Sorry 16bit audio it's your turn now, your going to be cut down to 12bit to fit into a 24bit circle.<br>

In any scenario, I have successfully accomplished my goal. I now have the worlds best Professional High Resolution Audio Player, brought to you by the number 24 Ah-Ah-Ah!<br>

Welcome to the headphone control center<br>

This is how I calculated the amount of channels for headphone & bluetooth<br>
There are 384 True Native Mode mixer paths<br>
384 X 4 = 1536 then 1536 X 4 = 6144<br>

This is how I calculated the kilohertz headphone & bluetooth<br>
44.1 X 4 = 176.4<br>

This is how I calculated the bit-rate headphone & bluetooth<br>
24 X 4 = 96<br>

Welcome to the QuadDAC control center<br>

This is how I calculated the amount of channels for speaker aka QuadDAC<br>
6144 X 4 = 24576<br>

This is how I calculated the kilohertz for speaker aka QuadDAC<br>
176.4 X 4 = 705.6<br>

This is how I calculated the bit rate for speaker aka QuadDAC<br>
96 X 4 = 384<br>

Welcome to the QuadDAC direct output<br>

DAC 0 = low-range<br>
DAC 1 = mid-range<br>
DAC 2 = high-range<br>
DAC 3 = offload<br>

You must divide everything by 4 from the speaker settings<br>

speaker is set to channels: 24576<br>
24576 divided by 4 = 6144<br>

speaker is set to kilohertz: 705.6<br>
705.6 divided by 4 = 176.4<br>

speaker is set to bit rate: 384<br>
384 divided by 4 = 96<br>

### Will this True Native Mode code work on other Android phones other than the Lgv20?
I can't say for absolutely certain, I can say for certain that the True Native Mode code runs excellent, on both of my Lgv20's, my main phone DeGoogled and the spare one with Google intact both running Stock Oreo ezV2020 v1.0 Kernel.  Who knows this True Native Mode code may work universally across all QuadDACs on all Android phones. It's up to you guys to beta test this code, my job is all done, I just had to recreate the True Native Mode code and make it work. The LG V series of phones, will have the best chance of this True Native Mode code working. Also keep in mind that I officially got True Native Mode working in v169.1, on 01-17-24 phones manufactured after that date may have True Native Mode disabled on the QuadDAC chip.<br>

### I want to add this True Native Mode code, to my Android phone?
My theory is that the two files responsible for making this all happen are, audio_platform_info.xml and mixer_paths_tasha.xml. All the other files are associated with the Android mixer and are the left over reminisce of my previous attempts of trying to increase the audio quality on the Lgv20 without avail. Duplicate all the changes I made leaving intact your unique settings in your mixer_paths.xml file. This will take you some time, it took me months upon months to program 14,000 lines of code in the mixer_paths file. I made notes in both files, to help you along the way. This is not for the novice computer user. The mixer_paths file must have zero typos, zero mistakes, zero errors. The QuadDAC also needs Enable System wide QuadDAC support v8.2 aka build.prop audio tweaks.<br>

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

The mixer_paths.xml file must have zero duplicates, or your phone will not boot. This is how you can check:
<pre>
 uniq -d your_mixer_paths_file.xml
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
