# How To Modify ALYS DB_002 Into A More Complete Voicebank
### If you are looking for explanation on how to use the modified voicebank from this repo or what the files in this package are, please check [readme.md](readme.md)!
From here on, ALYS_DB_002_JPN will be referred to as DB_002, and ALYS_DB_001_JPN will be referred to as DB_001.

## Steps
1) Download DB_002 and DB_001
2) Locate Japanese recording script.pdf (from now on, referred to as JP script), it should be in either ALYS/doc/ALYS4AE or ALYS-DB-002-JPN/doc, depending on which repository you downloaded ALYS from
3) Take the contents of the 'mid' folder and move them into the ALYS_DB_002_JPN folder (up one level). Delete the 'mid' folder.
4) Open JP script in a PDF viewer and the ALYS_DB_002_JPN folder in file explorer.
5) Rename the .wav files according to the table in JP script. For example, "s001.wav" should be renamed "_だあだ.wav", "s002.wav" should be renamed "_だいだ.wav", etc (VCV banks often name the source files starting with an underscore: _ ). For those that can't type in hiragana, or those that want the source files to be named in roumaji, put underscores between each syllable: "s001.wav" becomes "_da_a_da.wav", "s002.wav" becomes "_da_i_da.wav", etc. This format should work with moresampler's auto VCV oto function. This is a very tedious thing to do, as you have to rename over 300 files. Once you're done, you will likely want to run it through moresampler's auto VCV, or configure the oto.ini yourself (If you want to skip steps 1-5, you can use the BASE voicebank instead).
6) Copy your modified voicebank into your UTAU voice folder. Also install DB_001 now if you haven't.
7) Figure out which samples are missing. As far as I know, there isn't an easy way to check which samples are needed. I usually plug-n-play some USTs to see which notes don't play - if you open Tools > Voice Bank Settings while a note is selected, it highlights the sample you had selected in the UST. If the sample highlighted isn't the same as the note you selected (or if the note doesn't play), the sample's missing.
8) Figure out which recordings from DB_001 correspond to the missing samples. You can do this by making a new UTAU project and making notes with the missing samples as lyrics. Load DB_001 and select each note one at a time. In Voice Bank Settings under "Name", it will say the name of the original file. Copy all of the original files into a new folder somewhere (Make sure you're copying the files from the E4 folder, those are the same pitch as DB_002's samples).
9) Open the copied files in an audio editor and cut them to only contain the missing syllable. For example, if the missing syllable is "a ゆ", then cut the "ya_ya_yi_ya_yu_ya_ye_y.wav" file to only contain ya and yu (remove the first 3 and last 4 syllables. it's better to cut around the existing continuous sample than make a new one from syllables that aren't spoken one after another), moresampler will auto-oto it into "a ゆ". Name the file "_やゆ.wav" or "_ya_yu.wav".
10) Put all of the new samples into the voicebank folder and run moresampler's oto function again (or re-do the oto).
11) Put the DB_002 folder in your UTAU voice folder if you haven't already. The bank is now usable. You may also want to delete duplicated oto entries (if you chose to rename the duplicate oto entries when you ran moresampler, you can just delete the oto entires that have a number at the end).

## Resources
[Original DBs](https://labs.phundrak.com/ALYS)
[moresampler 0.8.4 DL](https://cocoacacao.wixsite.com/cocoa/moresampler-archive)
[moresampler auto vcv tutorial](https://www.youtube.com/watch?v=QSDZBeFNPnc)