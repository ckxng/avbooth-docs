# Soundboard Setup

This document contains notes taken while setting up the simple profile.  Nothing on this page currently affects Sunday morning service.

## Input Channels

Vocal Inputs:

- consist of podium(+48V), packs, and handhelds
- take up the first 10 input channels
- have not been shaped for tone except for high pass filter and proximity effect compensation
- channel PEQs are set to notch out problematic feedback frequencies (which is different for podium, packs, and handhelds)
    - these EQs are ok for general and untrained use.  for Sunday morning worship, a proper vocal EQ should be laid on top of this baseline.  The tradeoff is that for any cuts that are reduced or moved (to improve tone), it increases the importance of proper mic handling to avoid feedback.
- compressor is set aggressively, so an energetic speaker can yell uncomfortably loud and just barely clip the center frequencies
- podium has a mild gate (with both high pass and low pass filters on the trigger) to minimize fidgiting noises on the podium surface
- all vocal inputs send to the de-esser fx 2 send and NOT the main mix or auxes

Computer

- audio input to ST1 from Mac
- routes to main mix and auxes

ST3 In

- 1/4 stereo jack (with 1/8in st jack dongle) on the console surface
- routes to ST3 In
- routes to main mix and auxes

Ceiling Mics

- routes to two mono inputs
- condenser mics with phantom power
- routes to auxes only
- added to Ceilng DCA 1, so both levels can be controlled from one fader

## FX

Reverb Fx 1

- recieves signals from handhelds 3-5, colored blue on the board
- applies choral reverb effect
- returns via. reverb fx 1 return to main mix and auxes

De-Esser Fx 2

- recieves signals from vocal inputs
- applies de-essing
- returns via. de-esser fx 2 return to the main mix and auxes

Dynamic EQ Fx 3

- currently investigating whether a dynamic EQ will allow someone like tom to speak normally into his mic and use it for singing at the same time
- this will likely not be included in the actual "simple" profile, it's an experiment which might find use in the church profile

## USB

- all vocal channels, Ceiling L, Ceiling R, Main LR, Aux 1, Aux 2 are patched to USB
- setup for multi-channel recording at 96kHz
- recorded vocal channels, ceiling L, and ceiling R are patched for USB playback as back into their original inputs
- this makes it possible to capture a worship service and refine EQ and other settings at a later date

## Main Mix EQ

- Graphic EQ is barely used.
- Paremetric EQ was set by pumping pink noise and measuring from the back of the house, cutting peaks.
- Out via MainLR to amps and speakers

## Web Aux 1

- Flat EQ.
- Currently Stereo out the Streaming PC, but there is a slight hiss.  Switching to balanced XLR out to a USB audio interface on the Streaming PC.

## Foyer Aux 2

- Flat EQ.
- Unverified, but it is assumed that this goes out to a 70V PA amp.

## Issues

still considering the impact of these things...

- with all vocals going into the deesser, ones loses the ability to mix per aux.
    - with auxes being post-fade now, that's not as big an impact as it would have been.  need to listen to the web and foyer output to get a sense for how it sounds.
    - alternative will be to only put the podium and packs into the deesser, and leave the handhelds all independant for more mixer control.

[<- back](README.md)
