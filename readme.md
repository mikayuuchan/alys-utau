# ALYS DB_002 JPN - Modified UTAU Voicebank
## Info
This is a modified version of the [ALYS_DB_002_JPN voicebank](https://labs.phundrak.com/ALYS), configured as a VCV voicebank for [UTAU](http://utau2008.xrea.jp/).
The original voice DB does not contain enough samples to create a full VCV voicebank, so some samples were taken from the ALYS_DB_001_JPN bank (E4 pitch) to compensate.
From here on, ALYS_DB_002_JPN will be referred to as DB_002, and ALYS_DB_001_JPN will be referred to as DB_001.

Voice files from the mid-high and mid-low folders are not configured as working pitches, as there are far too few samples to make a working voicebank. This voicebank only contains the source files from the mid pitch. An icon for UTAU, a readme.txt, and an edited character.txt are included. The oto was automatically configured by moresampler 0.8.4. As such, it is not perfect, but functional. Because the oto is auto-generated, many oto entries have extras (like - あ２, o ら2, etc) so if a sample does not sound very good, you may want to try an alternate one.
 
## Included Files
### Two versions of the voicebank, and one extra folder:
#### ALYS_DB_002_JPN_UTAU_BASE:
Files renamed to match recording list, no extra samples. This voicebank is the closest to the original DB, and has an oto. Use it if you don't want the extra samples taken from DB_001, or want to add them yourself. This voicebank contains about 70-80% of what a full VCV voicebank needs, so it won't plug and play VCV .USTs well.
#### ALYS_DB_002_JPN_UTAU_COMPLETE:
Files renamed, extra samples included. It may not have 100% of the samples needed for full VCV, but it should be very close. This is the recommended one to use if you just want a working version of DB_002.
#### EXTRA: 
##### ADDED_SAMPLES:
The new samples taken from DB_001. This is just a copy of them for playing around with or looking at.
##### C4/G4:
Renamed mid-low and mid-high pitches to match the recording script. There is very little here, but I thought I'd include it anyways.
##### alys demo ust:
A quick ust showing off ALYS's vcv capabilities and vocal range.

For those looking to try their hand at improving this voicebank or making their own modified version of the original DB_002, please take a look at [how-to.md](how-to.md).

## Voicebank Usage Tips
Recommended resampler is moresampler. ALYS has very slow consonants, so a high consonant velocity will help her a lot.

This voicebank is available under the GPL-3.0 license.

## Resources
- [Original DBs](https://labs.phundrak.com/ALYS)
- [moresampler 0.8.4 DL](https://cocoacacao.wixsite.com/cocoa/moresampler-archive)
- [moresampler auto vcv tutorial](https://www.youtube.com/watch?v=QSDZBeFNPnc)

## Contact
If you have any questions, troubleshooting issues, or find missing samples I overlooked, feel free to DM or @ me on [Twitter](https://twitter.com/mikayuu_chan), send an ask or message me on [Tumblr](https://mikayuu-chann.tumblr.com/), or create an issue or pull request on the github repo.