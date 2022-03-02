Stream Punk's Bitwig Presets
============================

Addiktone
---------

An easy, airy additive synthesizer. There is almost no setting that doesn't
work, while you can produce unique, rich and sometimes slightly dented sounds.
By default it pulls many stereo tricks and has a very wide image. The rich
overtones make it very present, but you can tone it down so it plays nicely in
the background.

The overtones create a randomized moving shape, you can change the amount with
the `Moving` knob. The overtones are slightly panned and moving in the stereo
image, controlled by the `Spread` knob. If you turn the `Random` knob down, the
shape of the overtones repeats and becomes deterministic. Turn it all the way up
for maximum blessings from the god of `Dices`.

The main sound-shaping comes from `Skew`, `Fold`, `Detune` and `Follow`. If you
know the `Poly Grid` these are no strangers to you. Just twist those knobs,
you'll get the hang it easily.

Then there is your standard envelope-controlled, key-tracked low-pass filter
and a `Multinote` device playing a fifth for maximum richness.

https://youtu.be/qJ284O69YeQ

Note Mode
---------

Change the mode of multiple tracks with one global track. The keys notes
C,D,E,F,G,A,B (0,1,2,3,4,5,6) select the mode-shift using Bitwig's `Key Filter`
device. The device `Note Mode Output` is placed in the global mode-track. It
sends the mode via `MIDI-CC 20`. In the tracks you want to change the mode, you
place the `Note Mode Input` device in front of the instruments. You have to open
the chain of `Note Mode Input` and select the global mode-track.

There is also the `Note Mode Shift`-preset which allows you to automate the
mode-shift locally in one track.

Note Modulo
-----------

When using the `Note Mode` devices it is helpful when an octave wraps around, so
shifting the mode does not pitch the melody or chord too high. If you are
shifting chords, you can think of `Note Modulo` as inversions.

General MIDI Drums
------------------

There is a submodule containing General MIDI Drums. These are converted from a
open [General MIDI soundfont](https://schristiancollins.com/generaluser.php).
The licensing of the orginal work applies.

Get the submodule with

```bash
git submodule update --init --recursive
```
