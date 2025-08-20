title: Improvements to Digital Vinyl Control
authors: Owen Williams
tags: community, contribute, development, announcement
comments: yes

Everything old is new again, trends keep coming back around, and that goes doubly so for the venerable DJ turntable.

Mixxx has supported vinyl control for many years, and was one of the first major rewrites I did for the Mixxx project when I first joined back in 2009.
However, over the years the code has rotted, bugs have appeared, and mistakes I made more than 15 years ago have been a source of frustration for DJs wanting to use their turntable with Mixxx.
With the recent resurgent popularity of turntable-based DJing, that old code has gotten new attention, and we're proud to announce a major improvement in Mixxx's vinyl performance, as well as the first open source implementation of Native Instruments' Traktor MK2 Control Vinyl.

## Sticker Drift

While Mixxx has performed well enough for basic two-deck mixing, it has not been accurate enough for high-intensity scratching.
The bane of any turntablist's existence is **sticker drift**.
Briefly, when a turntablist wants to scratch over a specific sound, that sound needs to be heard on the same physical spot on the record every single time.
If Mixxx's tracking is imprecise, that location will "drift", making it impossible to scratch or rewind accurately.

Sources of sticker drift in Mixxx were plentiful.
Our signal smoothing is now much more accurate, resulting in far less noise and jitter in the timecode signal.
And with a rock-solid signal, there's no need for the other hacks and workarounds that were added on top to "hide" these problems.
The result is a responsive, near-drift-free experience.

## Traktor Control Vinyl MK2

Thanks to [Jan's groundbreaking work](TKTKTKTK), Mixxx now has experimental support for Traktor Control Vinyl MK2.
For many years, Mixxx has only supported version 1 of Traktor's control vinyl, and that version has not been sold in stores for many years.
With this new code, DJs can finally use their Traktor control vinyl on an open source system.

## Feedback Wanted

Even with all the attention the vinyl code has gotten over the past few weeks, there is still a lot of testing to do.
We welcome feedback, bug reports, and feature requests from vinyl DJs about ways we can make Mixxx's vinyl control even better.
There are many combinations of sound cards and turntables, and we can only test the equipment we have.
[Please Get Involved!](https://mixxx.org/get-involved/)

## What's New in Vinyl Control

Here's a list of the major recent improvements to vinyl control in Mixxx:

- Fix vinyl control not initializing correctly on new installations (!)
- Vastly improve pitch tracking accuracy
- Fix pitch tracking at extreme speeds (rewinds)
- Remove unneeded smoothing post-processing that resulted in less responsiveness
- Add experimental support for Traktor Control Vinyl MK2
