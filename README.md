# CombinedAudioTool
- A Tool for CombinedAudio.bin for Minecraft for New Nintendo 3DS Edition (MC3DS) with a plethora of Features.
- Only support Windows Platforms Officially, due to being built and made using some Windows API functions.

## Feature Set:
- Extract All FSB Soundbank Files in the Archive.
- Extract a FSB Soundbank File by Name/Sound-ID.
- Get File name(s) from Soundbank Files for easier recognition.
- Rename Extracted files to original filename(s).
- Rebuild `CombinedAudio.bin` with new Custom Audio Files.
- Extract Header from `CombinedAudio.bin`.
- Add padding to files automatically (Requires Original Extracted File).
- Collect all Sound Names/ID's.
- Rename all Segments to Original Filenames.
- Grab Segment File Sizes individually, or altogether.
- Updating your Script as new features become avaliable.
- Extract Audio from FSB Files (now including GCADPCM FSB Soundbank Files).
- Convert `*.wav` back into GCADPCM/DSADPCM.
- Restore CATool File Integrity.
- Encode Minecraft 3DS Music Files from Wave Files.
- Convert any Audio Filetype to Wave.
- Install FFMPEG via Command Line.

## Download(s):
- Download [Here](https://github.com/Minecraft-3DS-Community/CombinedAudioTool/releases/download/v1.9/CATool.zip).
- Requires `Python 3.8+` and `Python STD` (Installed alongside Python).

## Usage:
```
python CATool.py
       --eca,  extract-ca     [CombinedAudioPATH]                            > Extracts All FSB Soundbank Files from the CombinedAudio.bin Archive.
       --fn,   find-sn        [SegmentFilePATH]                              > Find the Segment Name from an Extracted FSB Soundbank File via --eca Flag.
       --rs,   rename-s       [SegmentFilePATH]                              > Rename a Segment File FSB Soundbank File back to it's Original Filename.
       --gh,   get-header     [CombinedAudioPATH]                            > Extracts the Header from the CombinedAudio.bin Archive.
       --rca,  rebuild-ca     [SegmentOutFolderPATH]                         > Rebuilds the CombinedAudio.bin Archive via Segment Files.
       --ap,   add-padding    [OriginalFilePATH]       [ModifiedFilePATH]    > Adds padding to set the Modified File Equal to the Original File Size.
       --ne,   name-extract   [CombinedAudioPATH]      [Sound Name/ID]       > Extracts a FSB Soundbank File from the CombinedAudio.bin Archive via Name/SoundID.
       --ra,   rename-all     [SegmentFolderPATH]                            > Renames all Segment Files back to their original FSB Soundbank Filename(s).
       --gsid, get-soundid    [CombinedAudioPATH]                            > Gets all Sound Names/ID's and Dumps them to a *.txt File.
       --gssg, get-size-seg   [SegmentFilePATH]                              > Gets the size of a specific Segment Soundbank FSB File.
       --gs,   get-size       [SegmentOutFolderPATH]                         > Gets the size of all Segment Soundbank FSB Files.
       --exa,  extract-seg    [SegmentFilePATH]                              > Attempts to extract Audio from Segment Soundbank FSB Files.
       --cwav, convert-wave   [SegmentFilePATH]        [FileToConvertPATH]   > Convert Custom Audio to Nintendo 'GCADPCM'/'DSADPCM' Format (*.dsp).
       --pa,   play-audio     [WaveFilePATH]                                 > Play Audio from a Wave-File.
       --gsmc, generate-music [WaveFilePATH]                                 > Generates a Valid Music FSB Soundbank File for Minecraft 3DS Edition from a Wave File.
       --atw,  to-wave        [AudioFileToConvertToWavPATH]                  > Convert basically any Audio format like *.ogg or *.mp3 to Wave Format.
       --impg, inst-ffmpeg                                                   > Install FFMPEG to '.\extrcd\mpg\bin'.
       --upd,  update                                                        > Updates From Current Version to the Latest Version of 'CATool.py'.
       --rstr, restore                                                       > Basically an Emergancy Version of '--upd' that Wipes all Files from CATool and Reinstalls them.
       --h,    help                                                          > Displays this Message.
```
### Help Message:
```
python CATool.py --h
```
![image](https://github.com/Minecraft-3DS-Community/CombinedAudioTool/assets/78656905/7d2d4adb-6f45-4484-85ee-c519ad9058b7)

## Sound ID's
```
thunder1
thunder2
explode1
explode2
rain1
rain2
shimmerblock
fire_crackle2
add_item1
add_item2
add_item3
break1
break2
place1
place2
remove_item1
remove_item2
rotate_item1
rotate_item2
death1
death3
grow1
grow4
empty_lava1
empty_lava2
empty1
empty2
fill_lava1
fill_lava2
fill1
fill2
splash
fallbig
fallsmall
weak1
weak2
weak3
hit1
hit2
hit3
cloth1
cloth2
cloth3
grass1
grass2
grass3
gravel1
gravel2
gravel3
sand1
sand2
sand3
snow1
snow2
snow3
stone1
stone2
stone3
wood1
wood2
wood3
in
out
fire
ignite
lava
lavapop
water
base
death
hurt1
hurt2
hurt3
idle1
idle2
idle3
takeoff
breathe1
breathe2
death
hit1
hit2
hit3
fireball4
hurt1
hurt2
plop
say1
say2
say3
step1
step2
hurt1
hurt2
hurt3
say1
say2
say3
step1
step2
step3
milk1
death
say1
say2
say3
death
hit1
hit2
hit3
idle1
idle2
idle3
portal
portal2
scream1
scream2
scream3
stare
hit1
hit2
wings1
wings3
wings5
growl2
growl3
affectionate_scream
charge
death
moan1
moan2
moan3
scream1
scream2
scream3
ambient1
attack_loop
curse
elder_death
elder_hit1
elder_idle3
flop1
guardian_death
guardian_hit1
land_death
land_hit1
land_idle1
angry1
death1
death2
idle1
idle2
idle3
idle4
idle5
spit1
spit2
hurt1
hurt2
hurt3
eat1
eat2
eat3
step1
step2
step3
step4
step5
swag
angry1
armor
breathe1
breathe2
breathe3
death
angry1
angry2
death
hit1
hit2
hit3
idle1
idle2
idle3
eat1
eat2
eat3
gallop1
gallop2
gallop3
hit1
hit2
hit3
idle1
idle2
idle3
jump
land
leather
death
hit1
hit2
hit3
idle1
idle2
idle3
soft1
soft2
soft3
wood1
wood2
wood3
death
hit1
hit2
hit3
idle1
idle2
idle3
idle2
death1
hurt2
step4
throw
death
hit1
hit2
hit3
walk1
walk2
walk3
ambient1
ambient2
ambient5
close1
close3
death1
death2
hurt_close1
hurt_close2
hurt1
hurt2
hurt3
open2
open3
shoot1
shoot4
hit1
hit2
hit3
big1
big2
big3
jump1
jump2
jump3
small1
small2
small3
death
pig_boost
pig_boost
pig_boost
say1
say2
say3
step1
step2
step3
hurt1
hurt2
hurt3
hurt4
idle2
idle3
hop1
hop2
hop3
bunnymurder
say1
say2
say3
shear
step1
step2
step3
hit2
hit3
kill
say1
say2
say3
step1
step2
step3
death
hurt1
hurt2
hurt3
say1
say2
say3
step1
step2
step3
big1
big2
big3
small1
small2
small3
attack1
attack2
death1
death2
death3
hurt1
hurt2
hurt3
bow
death
say1
say2
say3
step1
step2
step3
ambient1
ambient2
death3
hurt1
hurt2
idle2
death1
hurt4
step3
death
haggle1
haggle3
hit1
hit2
hit3
idle1
idle2
idle3
no1
no2
yes1
yes2
death1
death2
hurt1
hurt2
hurt3
idle1
idle2
idle3
fangs
idle1
idle2
idle3
cast1
cast2
death1
death2
hurt1
hurt2
prepare_attack1
prepare_attack2
prepare_summon
prepare_wololo
idle1
idle2
death1
death2
hurt1
hurt2
charge1
charge2
ambient5
ambient1
ambient2
death1
death2
death3
hurt1
hurt2
hurt3
drink1
drink2
drink3
throw1
throw2
throw3
idle1
woodbreak
death
death1
shoot
spawn
bark1
bark2
bark3
death
growl1
growl2
hurt1
hurt2
hurt3
panting
shake
step1
step2
step3
whine
hiss1
hiss2
hitt1
hitt2
hitt3
meow1
meow2
meow3
purr1
purr2
purreow1
purreow2
idle1
idle4
idle1
idle2
step1
step2
warning1
warning2
hurt1
hurt2
death1
death2
death
hurt1
hurt2
remedy
unfect
say1
say2
step1
step2
step3
wood1
wood2
wood3
zpig1
zpig2
zpig3
zpigangry1
zpigangry2
zpigangry3
zpigdeath
zpighurt1
zpighurt2
say1
say2
say3
death
hurt1
hurt2
bass
bassattack
bd
harp
hat
pling
snare
portal
anvil_break
anvil_land
anvil_use
bowhit1
bowhit2
bowhit3
break
burp
chestclosed
chestopen
close
open
click
door_close
door_open
drink
eat1
eat2
eat3
fizz
fuse
glass1
glass2
glass3
levelup
orb
pop
pop2
swim1
swim3
swim4
hurt
toast
use_totem
camera1
camera2
camera3
ladder1
ladder2
ladder3
cloth1
cloth2
cloth3
grass1
grass2
grass3
gravel1
gravel2
gravel3
sand1
sand2
sand3
snow1
snow2
snow3
stone1
stone2
stone3
wood1
wood2
wood3
cloth1
cloth2
cloth3
grass1
grass2
grass3
gravel1
gravel2
gravel3
sand1
sand2
sand3
snow1
snow2
snow3
stone1
stone2
stone3
wood1
wood2
wood3
```
