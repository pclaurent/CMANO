+---------------------------+
+ Command Talk Readme file  +
+ (c) Philippe Laurent 2019 +
+ laurizon@free.fr          +
+---------------------------+

Command Talk is an addon for Command Modern Air Naval Operations (CMANO). It
provides an audio environment by checking the game log and reading some of its
contents as if it was read by an actual sub/ship crew member (mainly the sonar
man). Some background noises are also added.

Command Talk has been greatly inspired by SeaHag. Thanks to the author.

Pre-requisite
-------------

Command Talk uses the .Net library (2017). Make sure you installed it from
Microsoft's website.

Installation
------------

Downlad the main file AND the language file.

Unzip the main zip files into the directory of your choice.

Copy the language sound files in the same directory.

Instructions
------------

It is mandatory to run CMANO and the scenario first, as Command Talk always reads
the latest generated log. So launch the scenario, wait around 15 seconds and then
only, doube-click on CommandTalk.exe (or press Start after this delay).

The interface is quite simple. First, select the directory containing the CMANO
logs (by default : "C:\Program Files (x86)\Steam\steamapps\common\Command Modern
Air Naval Operations\Logs"). Once selected, you will not need to select it again
in future runs of Command Talk.

Pressing the Start button starts the reading from the beginning of the log. If you
cannot hear anything, press Stop and then Start again. The reading will start at
the first event written in the log and the log flushed on disk by CMANO, so it can
take some time...

After the first run, a CommandTalk.ini file is created with some default values.
The first line contains the Logs path. The second line contains the key words
preceding the side name of the player. The following lines contain the keywords
to be found in the log and, the line after, the name of the sound file to be
played for each.

Default English sound files are recorded with a synthetic voice. You can record
your own natural voices instead to get a better game experience.

Some tips if you want to edit the CommandTalk.ini file (adding you own sequences
of key words for instance):

1. The order of appearance of keys does matter. Once a key is detected in the log,
   no other match will be searched for at the same position (but other keys will be
   checked for in the rest of the line).

2. @ stands for numerical value. These values will be spelled digit after digit.

You can of course add your own keyword lines and audio files. The "radioxx.wav"
files are just radio gibberish clips. You can replace them with other sound samples,
but their number must always be 15, no more, no less...
