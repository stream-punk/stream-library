Stream Punk's Bitwig Presets
============================

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
