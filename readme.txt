all files are located in
/system/vendor/etc/


I have calculated that a QuadDAC needs to have 288 mixer paths to function in True Native Mode. 144 on the headphone side and 144 on the speaker or DAC side for a total of 288. Each one mid-range, treble and bass requires 8 mixer paths to function. 8 X 3 = 24 for a QuadDAC you want to times that by six 24 X 6 = 144 then 144 X 2 = 288

For a DAC that has 8 cores you would timex that by 12 and so on.

The two main files that from my understanding that made this all possible would be 
audio_platform_info.xml
mixer_paths_tasha.xml

I disconnected the DAC from the phones mixer in file audio_platform_info.xml I programed the DAC for True Native Mode in file mixer_paths_tasha.xml

Your welcome to look over all my notes in the mixer_paths_tasha.xml and audio_platform_info.xml files, my hope is by documenting all the modifications I made is to have people reprogram other Android phones so everyone can enjoy Hi-Res audio.

I programed everything to upsample audio played at 44.1kHz.

I made three diffrent versions of Lemon Drop Hi-Res but only one souce code. To change the DAC modes search for: <path name="speaker-initialization-switch">


treble
	<ctl name="SpkrLeft COMP Switch" value="1" />
	<ctl name="SpkrLeft BOOST Switch" value="0" />
	<ctl name="SpkrLeft VISENSE Switch" value="0" />
	<ctl name="SpkrLeft WSA PA Mute" value="0" />
	<ctl name="SpkrLeft SWR DAC_Port Switch" value="1" />
	<ctl name="SpkrRight COMP Switch" value="1" />
	<ctl name="SpkrRight BOOST Switch" value="0" />
	<ctl name="SpkrRight VISENSE Switch" value="0" />
	<ctl name="SpkrRight WSA PA Mute" value="0" />
	<ctl name="SpkrRight SWR DAC_Port Switch" value="1" />

bass
	<ctl name="SpkrLeft COMP Switch" value="1" />
	<ctl name="SpkrLeft BOOST Switch" value="1" />
	<ctl name="SpkrLeft VISENSE Switch" value="0" />
	<ctl name="SpkrLeft WSA PA Mute" value="0" />
	<ctl name="SpkrLeft SWR DAC_Port Switch" value="1" />
	<ctl name="SpkrRight COMP Switch" value="1" />
	<ctl name="SpkrRight BOOST Switch" value="1" />
	<ctl name="SpkrRight VISENSE Switch" value="0" />
	<ctl name="SpkrRight WSA PA Mute" value="0" />
	<ctl name="SpkrRight SWR DAC_Port Switch" value="1" />

bass+
	<ctl name="SpkrLeft COMP Switch" value="1" />
	<ctl name="SpkrLeft BOOST Switch" value="1" />
	<ctl name="SpkrLeft VISENSE Switch" value="1" />
	<ctl name="SpkrLeft WSA PA Mute" value="0" />
	<ctl name="SpkrLeft SWR DAC_Port Switch" value="1" />
	<ctl name="SpkrRight COMP Switch" value="1" />
	<ctl name="SpkrRight BOOST Switch" value="1" />
	<ctl name="SpkrRight VISENSE Switch" value="1" />
	<ctl name="SpkrRight WSA PA Mute" value="0" />
	<ctl name="SpkrRight SWR DAC_Port Switch" value="1" />


