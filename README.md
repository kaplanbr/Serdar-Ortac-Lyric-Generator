# Serdar-Ortac-Lyric-Generator

Markow Chain model for generating Serdar Ortaç lyrics. Levenshtein similarity is used for ryhmes. Model writes 4 lines with rhyme logic at each run.  

Example usage:

import os
os.chdir(r"..\serdarortac") #file containing lyrics

from serdarortac import *
idir = os.path.join(os.getcwd(),"lyrics")
ortac_fwprobdict, ortac_bwprobdict = readLyrics(idir)
print("Here's your Serdar Ortac lyrics:\n")
print(makeSerdarOrtac("", ortac_fwprobdict, ortac_bwprobdict))

Here's your Serdar Ortac lyrics:

 sıkı dur
 yaşanan hayal kurup dualar
 uyanır dururum yakalar
 eriyor gittin gideli güvenim 
