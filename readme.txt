all files are located in
/system/vendor/etc/


I have calculated that a QuadDAC needs to have 288 mixer paths to function in True Native Mode. 144 on the headphone side and 144 on the speaker or DAC side for a total of 288. Each one mid-range, treble and bass requires 8 mixer paths to function. 8 X 3 = 24 for a QuadDAC you want to times that by six 24 X 6 = 144 then 144 X 2 = 288

For a DAC that has 8 cores you would times that by 12 and so on.

When programing the mixer paths for a QuadDAC you want two DACs on TX and two on RX like this. This applys to everything but the The DAC initialization code it applys to how many DACs you wan to enable, for a QuadDAC number 4 = enable all 4 DACs.

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

I made four diffrent versions of Lemon Drop Hi-Res but only one souce code. To change the DAC modes search for: <path name="speaker-initialization-switch">


treble
	<ctl name="SpkrLeft COMP Switch" value="4" />
	<ctl name="SpkrLeft BOOST Switch" value="0" />
	<ctl name="SpkrLeft VISENSE Switch" value="0" />
	<ctl name="SpkrLeft WSA PA Mute" value="0" />
	<ctl name="SpkrLeft SWR DAC_Port Switch" value="4" />
	<ctl name="SpkrRight COMP Switch" value="4" />
	<ctl name="SpkrRight BOOST Switch" value="0" />
	<ctl name="SpkrRight VISENSE Switch" value="0" />
	<ctl name="SpkrRight WSA PA Mute" value="0" />
	<ctl name="SpkrRight SWR DAC_Port Switch" value="4" />

bass+
	<ctl name="SpkrLeft COMP Switch" value="4" />
	<ctl name="SpkrLeft BOOST Switch" value="4" />
	<ctl name="SpkrLeft VISENSE Switch" value="4" />
	<ctl name="SpkrLeft WSA PA Mute" value="0" />
	<ctl name="SpkrLeft SWR DAC_Port Switch" value="4" />
	<ctl name="SpkrRight COMP Switch" value="4" />
	<ctl name="SpkrRight BOOST Switch" value="4" />
	<ctl name="SpkrRight VISENSE Switch" value="4" />
	<ctl name="SpkrRight WSA PA Mute" value="0" />
	<ctl name="SpkrRight SWR DAC_Port Switch" value="4" />


To change from the OC flavor or NOC flavor.

	<!-- Welcome to the Saber ESS 9218 QuadDAC direct output -->
	<!-- DAC 0 treble -->
	<!-- DAC 1 bass -->
	<!-- DAC 2 treble -->
	<!-- DAC 3 mid-range -->
	<!-- My understanding is DAC 0 and 2 has more power -->
	<!-- That's why I have treble on 0 and 2 -->
	<!-- There are 144 channels going to each DAC -->
	<!-- 144 X 4 = 576 and times that by eight 576 X 8 = 4608 divide 4608 by 4 = 1152 per DAC total channels 4608 -->
	
	<path name="dop-playback tert-mi2s-headphones">
	<ctl name="SEC_TDM_TX_0 Audio Mixer MultiMedia5" value="2" />
	<ctl name="SEC_TDM_RX_0 Audio Mixer MultiMedia5" value="2" />
	<ctl name="SEC_TDM_TX_0 Channels" value="Onethousandonehundredfiftytwo" />
	<ctl name="SEC_TDM_RX_0 Channels" value="Onethousandonehundredfiftytwo" />
	<ctl name="SEC_TDM_TX_0 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_RX_0 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_TX_0 Format" value="S32_LE" />
	<ctl name="SEC_TDM_RX_0 Format" value="S32_LE" />
	<ctl name="SEC_TDM_TX_1 Audio Mixer MultiMedia1" value="2" />
	<ctl name="SEC_TDM_RX_1 Audio Mixer MultiMedia1" value="2" />
	<ctl name="SEC_TDM_TX_1 Channels" value="Onethousandonehundredfiftytwo" />
	<ctl name="SEC_TDM_RX_1 Channels" value="Onethousandonehundredfiftytwo" />
	<ctl name="SEC_TDM_TX_1 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_RX_1 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_TX_1 Format" value="S32_LE" />
	<ctl name="SEC_TDM_RX_1 Format" value="S32_LE" />
	<ctl name="SEC_TDM_TX_2 Audio Mixer MultiMedia5" value="2" />
	<ctl name="SEC_TDM_RX_2 Audio Mixer MultiMedia5" value="2" />
	<ctl name="SEC_TDM_TX_2 Channels" value="Onethousandonehundredfiftytwo" />
	<ctl name="SEC_TDM_RX_2 Channels" value="Onethousandonehundredfiftytwo" />
	<ctl name="SEC_TDM_TX_2 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_RX_2 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_TX_2 Format" value="S32_LE" />
	<ctl name="SEC_TDM_RX_2 Format" value="S32_LE" />
	<ctl name="SEC_TDM_TX_3 Audio Mixer MultiMedia3" value="2" />
	<ctl name="SEC_TDM_RX_3 Audio Mixer MultiMedia3" value="2" />
	<ctl name="SEC_TDM_TX_3 Channels" value="Onethousandonehundredfiftytwo" />
	<ctl name="SEC_TDM_RX_3 Channels" value="Onethousandonehundredfiftytwo" />
	<ctl name="SEC_TDM_TX_3 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_RX_3 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_TX_3 Format" value="S32_LE" />
	<ctl name="SEC_TDM_RX_3 Format" value="S32_LE" />
	</path>



	<!-- Welcome to the Saber ESS 9218 QuadDAC direct output -->
	<!-- DAC 0 treble -->
	<!-- DAC 1 bass -->
	<!-- DAC 2 treble -->
	<!-- DAC 3 mid-range -->
	<!-- My understanding is DAC 0 and 2 has more power -->
	<!-- That's why I have treble on 0 and 2 -->
	<!-- There are 144 channels going to each DAC -->
	<!-- 144 X 4 = 576 total channels -->
	
	<path name="dop-playback tert-mi2s-headphones">
	<ctl name="SEC_TDM_TX_0 Audio Mixer MultiMedia5" value="2" />
	<ctl name="SEC_TDM_RX_0 Audio Mixer MultiMedia5" value="2" />
	<ctl name="SEC_TDM_TX_0 Channels" value="Onehundredfortyfour" />
	<ctl name="SEC_TDM_RX_0 Channels" value="Onehundredfortyfour" />
	<ctl name="SEC_TDM_TX_0 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_RX_0 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_TX_0 Format" value="S32_LE" />
	<ctl name="SEC_TDM_RX_0 Format" value="S32_LE" />
	<ctl name="SEC_TDM_TX_1 Audio Mixer MultiMedia1" value="2" />
	<ctl name="SEC_TDM_RX_1 Audio Mixer MultiMedia1" value="2" />
	<ctl name="SEC_TDM_TX_1 Channels" value="Onehundredfortyfour" />
	<ctl name="SEC_TDM_RX_1 Channels" value="Onehundredfortyfour" />
	<ctl name="SEC_TDM_TX_1 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_RX_1 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_TX_1 Format" value="S32_LE" />
	<ctl name="SEC_TDM_RX_1 Format" value="S32_LE" />
	<ctl name="SEC_TDM_TX_2 Audio Mixer MultiMedia5" value="2" />
	<ctl name="SEC_TDM_RX_2 Audio Mixer MultiMedia5" value="2" />
	<ctl name="SEC_TDM_TX_2 Channels" value="Onehundredfortyfour" />
	<ctl name="SEC_TDM_RX_2 Channels" value="Onehundredfortyfour" />
	<ctl name="SEC_TDM_TX_2 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_RX_2 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_TX_2 Format" value="S32_LE" />
	<ctl name="SEC_TDM_RX_2 Format" value="S32_LE" />
	<ctl name="SEC_TDM_TX_3 Audio Mixer MultiMedia3" value="2" />
	<ctl name="SEC_TDM_RX_3 Audio Mixer MultiMedia3" value="2" />
	<ctl name="SEC_TDM_TX_3 Channels" value="Onehundredfortyfour" />
	<ctl name="SEC_TDM_RX_3 Channels" value="Onehundredfortyfour" />
	<ctl name="SEC_TDM_TX_3 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_RX_3 SampleRate" value="KHZ_352P8" />
	<ctl name="SEC_TDM_TX_3 Format" value="S32_LE" />
	<ctl name="SEC_TDM_RX_3 Format" value="S32_LE" />
	</path>



