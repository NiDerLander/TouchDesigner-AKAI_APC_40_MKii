TouchDesigner099 - AKAI APC 40 MKii

Tested and Developped on Windows 10 64-Bit Build 2020-22080
Midi mapping for the AKAI APC 40 MKii

This is the mkii version of this project - https://github.com/dagelabi/TouchDesigner-AKAI_APC_40_MK1

Features
Set the device mode ( Generic, Ableton or Alternate Ableton )
See the Communications Protocol Documentation page 10
All buttons, sliders and knobs are mapped, except [A|B] track buttons (they have three states, sot not sure how to do them yet)

How to use
Import the .tox into : /local/midi/userdevices
Open the MIDI Device Mapper
Create a new mapping
In the MIDI Map dropdown, select AKAI APC 40 MKii
Select the device mode in /local/midi/userdevices/AKAI_APC_40_MK2/Setup
The CHOP channels are named :
{type}{channel}_{index}_{name}

Example :
Button : b2_61_device_control_prev
Slider/Faders : s1_49_track_control

Note:
[Track Select] buttons do not sends dedicated CC in "User" mode. Instead, thay send values of eight device control knobs for corresponding track. In "Ableton Live" and "Alternate Ableton Live" modes they sends own CCs, and do not send values of device control knobs. 

To do
Not sure yet, maybe will expand functionality later

Ref
Communications Protocol Documentation : https://www.akaipro.com/amfile/file/download/file/495/product/15/
