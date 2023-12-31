all files are located in
/system/vendor/etc/


This is how I calculated the amount of mixer paths to program in for True Native Mode for the QuadDAC. Bass, mid-range and treble all require 16 mixer paths each for a QuadDAC. So 16 X 3 = 48 then for a QuadDAC you want to times 48 X 16 = 768. So 768 is our magic number.


When programing the mixer paths for a QuadDAC you want two DACs on TX and two on RX like this. This applies to everything. Because you have a left and right channel or TX or RX and you do not want all 4 DACs working on the same thing and the same time.

	<ctl name="RX INT6 SPLINE MIX LO4 Native Switch" value="2" />
	<ctl name="RX INT6 SPLINE MIX LO4 Switch" value="2" />
	<ctl name="RX INT9 SPLINE MIX MI5 Native Switch" value="2" />
	<ctl name="RX INT9 SPLINE MIX MI5 Switch" value="2" />
	<ctl name="RX INT10 SPLINE MIX HI6 Native Switch" value="2" />
	<ctl name="RX INT10 SPLINE MIX HI6 Switch" value="2" />
	<ctl name="TX INT11 SPLINE MIX LO7 Native Switch" value="2" />
	<ctl name="TX INT11 SPLINE MIX LO7 Switch" value="2" />
	<ctl name="TX INT12 SPLINE MIX MI8 Native Switch" value="2" />
	<ctl name="TX INT12 SPLINE MIX MI8 Switch" value="2" />
	<ctl name="TX INT13 SPLINE MIX HI9 Native Switch" value="2" />
	<ctl name="TX INT13 SPLINE MIX HI9 Switch" value="2" />

The two main files that from my understanding that made this all possible would be 
audio_platform_info.xml
mixer_paths_tasha.xml

I disconnected the DAC from the phones mixer in file audio_platform_info.xml I programed the DAC for True Native Mode in file mixer_paths_tasha.xml

Your welcome to look over all my notes in the mixer_paths_tasha.xml and audio_platform_info.xml files, my hope is by documenting all the modifications I made is to have people reprogram other Android phones so everyone can enjoy Hi-Res audio.

I programed everything to upsample audio played at 44.1kHz.

I made two diffrent flavors of Lemon Drop Hi-Res but only one souce code. To change the DAC modes search for: <path name="speaker-initialization-switch">


treble
	<ctl name="SpkrLeft COMP Switch" value="2" />
	<ctl name="SpkrLeft BOOST Switch" value="0" />
	<ctl name="SpkrLeft VISENSE Switch" value="0" />
	<ctl name="SpkrLeft WSA PA Mute" value="0" />
	<ctl name="SpkrLeft SWR DAC_Port Switch" value="2" />
	<ctl name="SpkrRight COMP Switch" value="2" />
	<ctl name="SpkrRight BOOST Switch" value="0" />
	<ctl name="SpkrRight VISENSE Switch" value="0" />
	<ctl name="SpkrRight WSA PA Mute" value="0" />
	<ctl name="SpkrRight SWR DAC_Port Switch" value="2" />

bass+
	<ctl name="SpkrLeft COMP Switch" value="2" />
	<ctl name="SpkrLeft BOOST Switch" value="2" />
	<ctl name="SpkrLeft VISENSE Switch" value="2" />
	<ctl name="SpkrLeft WSA PA Mute" value="0" />
	<ctl name="SpkrLeft SWR DAC_Port Switch" value="2" />
	<ctl name="SpkrRight COMP Switch" value="2" />
	<ctl name="SpkrRight BOOST Switch" value="2" />
	<ctl name="SpkrRight VISENSE Switch" value="2" />
	<ctl name="SpkrRight WSA PA Mute" value="0" />
	<ctl name="SpkrRight SWR DAC_Port Switch" value="2" />
