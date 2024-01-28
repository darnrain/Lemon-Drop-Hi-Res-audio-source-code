![294729981-1fd80758-cdef-4be1-afb5-1d6666d383a0](https://github.com/darnrain/Lemon-Drop-Hi-Res-audio-source-code/assets/60840489/c7f73ce2-8e2e-4c9c-955c-38dced1bd54c)
## Lemon Drop Hi-Res audio source code

Welcome to the future of music...<br>
The Lgv20 was first with the Android Nougat operating system.<br>
Now it's the first running in True Native Mode.<br>
With all 4 DACs enabled.<br>
v184.1 or higher has the absolute maximum values of 2048bit, 5644.8kHz and 786432 channels.<br>

Please listen at a safe volume level.<br>

Lemon Drop Hi-Res development status: Active.<br>
latest release: v184.1<br>

In my professional opinion, I only recommend using v184.1 or higher. If you keep trying, odds are eventually you will succeed.<br>

### Introduction:
First off I want to say, I try to keep my writing to rated PG. (pretty good) Also I do have a very good sense of humour. I never understood why some people are serious all the time, life's too short for that.<br>

If you all were wondering why I left XDA, I will tell you. It's because these LineageOS devs were telling people that "I suck at programing and do not use Lemon Drop HI-Res, it will drain your battery", saying everything they can to try and discourage people from using Lemon Drop Hi-Res. It actually doesn't bother me one iota, if not a single person out there wants to use Lemon Drop Hi-Res, I designed and created Lemon Drop Hi-Res entirely for me and me alone. I like to share, that's just who I am. I absolutely love my Lgv20 and I don't plan on ever buying a new phone ever! The Lgv20 has everything and more I could ever ask for in a cell phone, not to mention a removable battery. If the Lgv20 did not have a removable battery, then I would have never created Lemon Drop Hi-Res. Why spend over 3+ years on a cell phone that has a non-replaceable battery? By the time I was done developing and creating Lemon Drop Hi-Res, most everyones battery would be ready to be replaced about the time I was done.<br>

Well I guess they found me again, I keep getting emails from comments on GitHub, telling me to "Please stop lying to people.". What does that even mean? They could be a little more descriptive in what they are attempting to convey. Why would I lie to people about programing a QuadDAC? The 18,000 lines of code that I have written, is in the mixer_paths_tasha.xml.modded file for everyone to see. Who knows, maybe they genuinely think I am trying to cause harm to peoples phones? That is absolutely not true. I just wanted to have a little fun programing a QuadDAC and increasing the audio quality on my Lgv20. After thinking about that last statement, that does sound kinda odd. I mean who even attempts to program a QuadDAC in there spare time? Furthermore is it even possible to program the QuadDAC on the Lgv20? Haha the answer is yes, if your good at programing code, math and you enjoy a good challenge. My 34 years of computer experience helps also. I suppose some people do have a hidden agenda, mine would be, I wanted to show off my advanced computer skills, and I wanted to own one of the only cell phones, that has the absolute best audio quality out of any cell phone in the entire world.<br>

As of a direct result of the harassment from the LineageOS devs, no one can open an issue or leave a comment on any of my projects on GitHub. It's fascinating to me how one little decision in life can and in some cases will have an extremely large outcome. I'm absolutely positive that True Native Mode would not be working yet. I need 100% uninterrupted total concentration, to program the QuadDAC. I cant have people telling me to stop liying, when I am on the precipice of one the greatest breakthroughs in the entire history of mankind.<br>

It's funny, but the LineageOS devs reminds me exactly of when your watching a movie and your just getting lost in the movie, then all of a suddenly out of nowhere, this HUGE fly shows up and wants to fly right in front of your face. Where's my certified, LineageOS dev fly swatter. lol<br>

### What is True Native Mode on a computer?
"(1) The normal running mode of a computer, executing programs from its built-in instruction set. Contrast with emulation mode. See native language. (2) The highest performance state of a computer."<br>

### What is True Native Mode on the Saber ESS 9218 DAC?<br>
I created all 4632 lines of the True Native Mode v3.0 code myself, with the help of sed, awk, echo, nano and l3afpad, there are 786 mixer paths for True Native Mode that places the QuadDAC into it's highest performance state. The very essence of True Native Mode it's self allows you to overclock the QuadDAC, v184.1 or higher has the absolute maximum values of 2048bit, 5644.8kHz and 786432 channels.<br>

### Is Lemon Drop Hi-Res audio source code still in the development stages?
Yes but with v184.1, I am getting very close to being all done.<br>

### How did you find this True Native Mode code?
If your curious on how I found the True Native Mode code, I will show you. Someone left about 0.5% of the code in the original mixer_paths_tasha.xml file for the Lgv20. Go to line number 278 through 287 you will see the 0.5% of the True Native Mode code that I found. As you can see, INI1 HPHL, INI2 HPHR, INI7 SPKRL, INI8 SPKRR, INI3 LO1, INI4 LO2, INI5 LO3, INI6 LO4, lines of code are partially there, the absolute perfect base starting point for me, to recreate the True Native Mode code. LO1 even started with INI3 that gave me my first clue. The other 99.5% I made with my own hands, all by myself. With trial and error and logic and my advanced Linux computer skills, if the code does not exist, make it yourself. No external resource was utilized, to my knowledge a resource of this nature absolutely does not exist. If you want to confirm that this original mixer_paths_tasha.xml is authentic, I will give you the link to the Lgv20 rom that has this 0.5% True Native Mode code.<br> https://androidfilehost.com/?fid=1322778262904012823

Update: I found the missing piece to the puzzle. Look in the original mixer_paths_tasha.xml. Line number: 549 - 552. That's so odd, it's almost like someone left bread crumbs deliberately for me to follow.<br>

### How did you transform the Lgv20 into A Professional High Resolution Audio Player?
34 years of advanced computer experience. Instead of a Nintendo my parents bought me a Commodore 64, that's how I learned how to write code. My very first computer was a vic 20, I don't count that computer because all I did was play games. The absolute most nostalgic game I have ever played as a kid, would have to be Space Invaders. I loved that game, still do to this day.<br>

### My music does not sound Overpowered sometimes?
Can be due to the following:<br>
1. The QuadDAC was not able to acquire the precise Ohm rating of your headphones, to fix unplug your headphones and plug them back in.<br>
2. The phone is in low power mode.<br>
3. Your battery is to low, it is undetermined on how much battery power we must have. I would say at least over 15%.<br>

### Did you tune this QuadDAC?
Yes I did, there are volume levels you can choose when programing the DAC, for bass, mid-range and treble. If they are all on the same volume level, then the audio will get all jumbled up. I was thinking when tuning the DAC, you want to hear the singer first and foremost and the bass in the background. The higher the number, the increased volume level of the audio. If you listen closely, you should be able to hear that your music has a sense of depth perception to it. I thought that would be extremely unparalleled.<br>

bass = volume level 51<br>
mid-range = volume level 53<br>
treble = volume level 55<br>

### How did you program and tune the QuadDAC?
When programing a QuadDAC you do not have visual gauges to view to see if you have done something wrong, its all done by the sound of the DAC. For example if you have increased the amount of channels way to high or messed up on your programing code, then the DACs volume will be decreased or the music will not sound like its full of life. The only way to accomplish that, is to lower the AVC volume. In other words it decreases the power to the DAC so you can program and tune the DAC. In v142.1 and higher the AVC volume is set to the maximum. To answer the question, I used my 34 years of advanced computer skills and used, awk, sed, echo and nano to create the True Native Mode code.

I was always seeing LO in the True Native Mode code. I was like what is LO??? Then it hit me it's the bass. I came up with MI and HI for mid-range and treble myself and it worked!!! Also I was always seeing RX everywhere I looked, I was like well if there is an RX there has to be a TX. I guess you could say it was trial, error, logic and my advanced Linux computer skills, is how I programed the Saber ESS 9218 DAC. The devs that programed the Saber ESS DAC chip are professionals, you need to think like how they think. They would not make it to complicated to program the QuadDAC. For me it is the ultimate puzzle.<br>

### How did you calculate the numbers?<br>
It’s so complex programing a QuadDAC, and it’s extremely complicated to setup everything correct. That’s what I have been trying to do. I’m done programing the QuadDAC. There are so many things that need to be setup with the correct numbers. I did it, I got everything setup correct in v184.1. I will explain what I did to achieve this.  v184.1 has the absolute maximum values of 2048bit, 5644.8kHz and 786432 channels. As you all know, I love a good challenge and let me tell you this was one of the challenging tasks that I have ever attempted.<br>

This is how I have the QuadDAC setup, I'm not entirely sure what offload is. I just know we need it, it's part of the QuadDAC. Without offload the music does not sound correct. So as you can see all 4 items have there own DAC, all 4 DACs play simultaneously. That's what is so unique about a QuadDAC, there is a huge amount of low-range & mid-range & high-range & offload all blasting away simultaneously. As apposed to a single DAC. In my failed experiments, I found that DAC 0 and DAC 2 have the most power, or volume level. That is why low-range and high-range are on those DACs.<br>

DAC 0 = low-range<br>
DAC 1 = mid-range<br>
DAC 2 = high-range<br>
DAC 3 = offload<br>

There are two sides that you need to set the correct amount of channels, the headphone side and the QuadDAC side. I will be talking about the headphone side. There are 384 True Native Mode mixer paths for each DAC, there are 4 DACs as you know. I had 1536 channels this entire time in all the past versions other than v184.1 or higher, when it should have been 3072 for stereo. We don’t want mono.<br>

I should also mention, 128 is the number I used to overclock the QuadDAC. When the QuadDAC is running in True Native Mode, it is possible  to overclock the QuadDAC.<br>

The number 128 could be because one of two things. If ask me, my money's on number one.<br>
1. The QuadDAC each DAC is 32bit 32 X 4 = 128<br>
2. There are 384 mixer path for True Native Mode, the prime numbers of 384 are: 64, 96, 128, 192<br>

This is the kilohertz<br>
44.1 X 128 = 5644.8<br>

This is the bit rate<br>
16 X 128 = 2048<br>

This is the QuadDAC direct output that I will be talking about. This is how I calculated the amount of channels<br>

There are 384 X 2 = 768 mixer paths for stereo<br>
You need to times 768 X 4 = 3072<br>
There are 3072 channels going to each DAC<br>
3072 X 128 = 393216 then divide 393216 by 2 = 196608 for a total of 786432 channels<br>
You want to divide 393216 by 2 because of stereo<br>

This was not easy to calculate, it took me many failed attempts before I got it right. If you keep trying, odds are eventually you will succeed.<br>

### Will this True Native Mode code work on other Android phones other than the Lgv20?
I can't say for absolutely certain, I can say for certain that the True Native Mode code runs excellent, on both of my Lgv20's, my main phone DeGoogled and the spare one with Google intact both running Stock Oreo ezV2020 v1.0 Kernel.  Who knows this True Native Mode code may work universally across all QuadDACs on all Android phones. It's up to you guys to beta test this code, my job is all done, I just had to recreate the True Native Mode code and make it work. The LG V series of phones, will have the best chance of this True Native Mode code working. Also keep in mind that I officially got True Native Mode working in v169.1, on 01-17-24 phones manufactured after that date may have True Native Mode disabled on the QuadDAC chip.<br>

### I want to add this True Native Mode code, to my Android phone?
It is my understanding that the two files responsible for making this all happen are, audio_platform_info.xml and mixer_paths_tasha.xml. This is only a theory, I am 99.9% positive, that you only need to mod those two files. All the other files are associated with the Android mixer and are the left over reminisce of my previous attempts of trying to increase the audio quality on the Lgv20 without avail. Duplicate all the changes I made leaving intact your unique settings in your mixer_paths.xml file. This will take you some time, it took me months upon months to program 14,000 lines of code in the mixer_paths file. I made notes in both files, to help you along the way. This is not for the novice computer user. The mixer_paths file must have zero typos, zero mistakes, zero errors. The QuadDAC also needs Enable System wide QuadDAC support v8.2 aka build.prop audio tweaks.<br>

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
