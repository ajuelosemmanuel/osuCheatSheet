# osu!CheatSheet

> A small website for a lot of osu! resources !
## Shortcuts

### General

+ `Alt + Up/Down Arrow` : Adjust volume
+ `Ctrl + Alt + Shift + S` : Reload skin
+ `Ctrl + O` : Options sidebar
+ `F8` : Open chat window
+ `F9` : Open extended chat window
+ `F10` : Toggle mouse buttons
+ `F12` : Take a screenshot

### Song select menu only

+ `Ctrl + 1/2/3/4` : Switch game mode to osu!/osu!taiko/osu!catch/osu!mania
+ `F1` : Open the game modifiers selection menu (mods)
+ `F2` : Select a random beatmap
+ `Shift + F2` : Go back to the previously random-selected beatmap (when you `F2` twice and skip a banger)
+ `Shift + Enter` : Open/Collapse a category (or collection)
+ `F3` : Open beatmap options menu
  + `1` : Manage collections
  + `2` : Delete
  + `3` : Remove from unplayed
  + `4` : Clear local scores
  + `5` : Edit
  + `6` : Cancel

### Game modifiers selection menu only
+ `Q` : EZ
+ `W` : NF
+ `E` : HT
+ `A` : HR
+ `S` : SD
+ `D` : DT
+ `F` : HD
+ `G` : FL
+ `Z` : RX
+ `X` : AP
+ `C` : SO
+ `V` : Auto
+ `B` : Sv2

## Searching beatmaps in-game (from the [wiki](https://osu.ppy.sh/wiki/en/Interface#search))

### Supported filters
+ `artist` : Name of the artist
+ `creator` : Name of the beatmap creator
+ `ar` : Approach Rate
+ `cs` : Circle Size
+ `od` : Overall Difficulty
+ `hp` : HP Drain Rate
+ `keys` : Number of keys (osu!mania and converted beatmaps only)
+ `stars` : Star Difficulty
+ `bpm` : Beats per minute
+ `length` : Length in seconds
+ `drain` : Drain Time in seconds
+ `mode` : Mode. Value can be `osu`, `taiko`, `catchthebeat`, or `mania`, or `o`/`t`/`c`/`m` for short.
+ `status` : Ranked status. Value can be `ranked`, `approved`, `pending`, `notsubmitted`, `unknown`, or `loved`, or `r`/`a`/`p`/`n`/`u`/`l` for short.
+ `played` : Time since last played in days
+ `unplayed` : Shows only unplayed maps. A comparison with no set value must be used. The comparison itself is ignored.
+ `speed` : Saved osu!mania scroll speed. Always 0 for unplayed maps or if the Remember osu!mania scroll speed per beatmap option is off

### Supported comparisons:

+ `= or ==` : Equal to
+ `!=` : Not equal to
+ `<` : Less than
+ `>` : Greater than
+ `<=` : Less than or equal to
+ `>=` : Greater than or equal to
You may also enter a difficulty or beatmap ID number in your search to get a single result.

## Multiplayer commands (from the [wiki](https://osu.ppy.sh/wiki/en/osu%21tourney/Tournament_Management_Commands))

+ `!mp make <name>` : Creates a tournament room with the specified name. A maximum of 4 such rooms may be created.
  + This room is special in that it is not closed when all players have left the room, and it is password protected from players joining this room themselves.
  + When the room is finished, use !mp close to close the room.
+ `!mp name <title>` : Updates the room name.
+ `!mp invite <username>` : Invites a player to the room.
  + Note that this does not bypass any private message blocks available in the osu! client, so your tournament staff will need to tell players to disable "Block private messages from non-friends" in the osu! options.
+ `!mp lock` : Locks the room so that players can’t change their team and slot.
+ `!mp unlock` : Reverses the above.
+ `!mp size <size>` : Sets the amount of available slots (1-16) in the room.
+ `!mp set <teammode> [<scoremode>] [<size>]` : Sets various room properties.
  + `teammode` : 0: Head To Head, 1: Tag Coop, 2: Team Vs, 3: Tag Team Vs
  + `scoremode` : 0: Score, 1: Accuracy, 2: Combo, 3: Score V2
+ `!mp move <username> <slot>` : Moves a player within the room to the specified 1-indexed slot.
+ `!mp host <username>` : Transfers host to the player.
+ `!mp clearhost` : Clears the room host.
+ `!mp settings` : Displays full room details.
+ `!mp start [<time>]` : Starts the match after a set time (in seconds) or instantaneously if time is not present.
+ `!mp abort` : Aborts the match.
+ `!mp team <username> <colour>` : Moves a player to the specified team.
  + `colour` : red, blue
+ `!mp map <mapid> [<playmode>]` : Changes the beatmap and playmode of the room.
  + `playmode` : 0: osu!, 1: Taiko, 2: Catch The Beat, 3: osu!Mania
+ `!mp mods <mod> [<mod>] [<mod>] …` : Removes all currently applied mods and applies these mods to the room.
  + Any amount of mods can be entered.
  + `mod` : HR, DT, FL, HD, FI, Freemod, None
+ `!mp timer [<time>]` : Begins a countdown timer.
  + `time` is 30s default.
  + Timer announcements occur every minute, 30s, 10s, 5s and earlier.
+ `!mp aborttimer` : Stops the current timer (both normal timers and match start timer)
+ `!mp kick <username>` : Kicks the player from the room.
+ `!mp password [<password>]` : Changes the password of the room. The password will be removed if <password> is not provided.
+ `!mp addref <username> [<username>] …` : Adds a referee to the room. A maximum of 8 referees may be added. Only the creator of the room can add a referee.
  + Referees must join the room in-game, or by entering the room's chat channel through `/join #mp_<room_id>` in IRC.
  + Referees can manage the room like the creator, however they cannot add or remove other referees themselves.
  + The [osu!tourney client](https://osu.ppy.sh/wiki/en/osu%21tourney) will show the room chat for referees.
+ `!mp removeref <username> [<username>] …` : Removes a referee from the room. Only the creator of the room can remove a referee.
+ `!mp listrefs` : Lists all referees in the room.
+ `!mp close` : Closes the room.
Sending `!mp help` to BanchoBot will reveal the commands.

Items enclosed within angle brackets ( `<>` ) define "parameters" of commands. Parameters enclosed within square brackets ( `[]` ) are optional. Usernames must have any whitespace be replaced with underscores ( `_` ). `#<userid>` may substitute `<username>` in all of the commands.

## Websites

+ [osu! official website](https://osu.ppy.sh/) : Official osu! website
+ [osu!stats](https://osustats.ppy.sh/) : Official stats website
+ [r/osugame](https://www.reddit.com/r/osugame/) : Official subreddit for osu!
+ [Osekai](https://osekai.net/) : Excellent and good looking osu! related website that has 3 main parts : one for [medals](https://osekai.net/medals/) which is very well documented, one for [alternative rankings](https://osekai.net/rankings/) and one for [older osu! versions](https://osekai.net/snapshots/).
+ [osu-pps](https://osu-pps.com/#/osu/maps) : The place where you can search pp farm maps for your farming needs !
+ [osu!acc](https://osuacc.atilo.sh/) : A tool that show you which plays are bringing your global accuracy down, and how much they are
+ [osu!search](https://osusearch.com/) : Advanced search for osu! beatmaps
+ [osu!track](https://ameobea.me/osutrack/) : More statistics !
+ [o!rdr](https://ordr.issou.best/#/) : upload and share your replays with your osr file and without using youtube/streamable
+ [osu!Collector](https://osucollector.com/) : share and download collections
+ [osu! Stamina Trainer](https://ojcastaneda.github.io/osu-stamina-trainer-web/#/) : bot that gives stamina oriented maps
+ [Beatconnect](https://beatconnect.io/) : osu! beatmaps mirror
+ [chimu.moe](https://chimu.moe/beatmaps) : osu! beatmaps mirror
+ [osu!skills](https://osuskills.com/) : Alternative way to measure skill, with rankings by skillset
+ [Country #1 leaderboard](https://snipe.huismetbenen.nl/) : Make sure to select the right country (Netherlands by default)
+ [SliderStudio](https://slider.little.moe/) : Online slider maker
+ [osu! matchmaking](https://oma.hwc.hr/) : 1v1 or 2v2 matchmaking system for osu!
+ [Look At My Score!](https://lookatmysco.re/) : Online (clean) scorepost maker

## Tools
+ [OpenTabletDriver](https://github.com/OpenTabletDriver/OpenTabletDriver) : Excellent tablet driver
+ [StreamCompanion](https://github.com/Piotrekol/StreamCompanion) : Stream overlay tool (really really great)
+ [gosumemory!](https://github.com/l3lackShark/gosumemory) : Stream overlay tool (used by Tuna and CPOL)
+ [KeyOverlay](https://github.com/Blondazz/KeyOverlay) : Good looking key overlay
+ [osu-trainer](https://github.com/FunOrange/osu-trainer) : Beatmap difficulty controls for osu!
+ [FL Practice diff maker](https://github.com/ssz7-ch2/OsuPracticeDiffMaker) : Practice diff maker, mainly for FL players
+ [Mapping Tools](https://mappingtools.github.io/) : All-in-one application for efficient and creative mapping in osu!
+ [osr2mp4](https://github.com/uyitroa/osr2mp4-app) : Application to convert replay files to video
+ [chat4osu](https://gitlab.com/hallowatcher/chat4osu) : IRC chat for osu! built for referees
+ [CollectionManager](https://github.com/Piotrekol/CollectionManager) : Collection manager for osu! - make sure to read the tutorial before using it
+ [ezpp!](https://github.com/oamaok/ezpp) : browser extension that displays pp values for a beatmap without downloading it
+ [osu! Miss Analyzer](https://github.com/ThereGoesMySanity/osuMissAnalyzer) : Program to analyze misses in a given osu! replay
+ [Circleguard](https://github.com/circleguard/circleguard) : Circleguard is a tool to help you analyze osu! replays. Either your own, or replays from someone you suspect is cheating
+ [storybrew](https://github.com/Damnae/storybrew) : Storyboard maker for osu!

## Tutorials / Guides
### Improvement
+ [osu! phd](https://youtu.be/uc99yWeP1h4) : In depth guide about what are the different skills in osu! and how those are tied to each other
+ [Korilaks's guide to improving in osu!](https://puu.sh/unB20/caee7b883d.pdf) : In depth guide about how to play in order to improve efficiently (covers all "skillsets")
+ [khz streaming guide](https://docs.google.com/document/d/1xbNwH_vN4O3azBYwua-Z_3GOAI2d-kV_EeE96aiRLBU/edit) : khz's guide to streaming - for context, he's a 3 digit player who's known for his speed and stamina skills ([video version](https://youtu.be/JFTlYOY4-e4))
+ [Spare's video about stamina and speed](https://youtu.be/yXdtbFNgCfY) : Spare's "guide" to streaming, covering stamina and speed. In case you don't know, he's a 2 digit player who's well rounded to say the least.
+ [Notes on Ryuk's advices on speed](https://docs.google.com/document/d/1l9JG6gLRDGEoQmqaEQbQSikfFNauxtQm3LfIxmdaadQ/preview?pru=AAABdKKFBjE*g-vO7cfw9fvhxrfFyLjS1A) : Advices on speed/streaming - how to build speed/fingercontrol, which technique/switches, ...
+ [FrenZ's video about consistency](https://youtu.be/eXQI4HzphlU)
+ [MBmasher's Q&A video on FL](https://youtu.be/1oQlPgRNo00) : Questions list is in description
+ [Verto's video on alternating](https://youtu.be/xx3e1NKrbWc)
+ [SpeedrunsSin's guide for Tap X Players](https://www.reddit.com/r/osugame/comments/ejlgph/ultimate_guide_tap_x_players/) : Tap X alt playstyle guide (Tobe style)
+ [AndrewRK's "Stop Lying to yourself in osu!" reddit post](https://www.reddit.com/r/osugame/comments/f3r1yf/stop_lying_to_yourself_in_osu/) : Probably one of the best "rant" post on osugame I've ever seen, and also the perfect answer to "how do I get better at the game"

### Everything Else
+ [Happystick's interview with Dr. Levi Harrison](https://www.reddit.com/r/osugame/comments/7wni1t/i_went_through_happysticks_interview_with_dr_levi/) : Advices regarding hand stretching in order to avoid pain/RSI
+ [Verto's first video on osu! terms](https://youtu.be/FIOsNK1JPcg) : learn the osu! slang
+ [Verto's second video on osu! terms](https://youtu.be/0rjB5GxsxGg)
+ [How to make a customized overlay for streaming](https://www.reddit.com/r/osugame/comments/ec0id3/how_to_make_an_autochanging_background_overlays/) : Guide to have a fully customized (Dynamic HP bar, custom PP counter, auto changing BG, ...) streaming overlay
+ [How to remove latency on osu!](https://www.reddit.com/r/osugame/comments/hqoakj/tutorial_removing_perceivable_latency_for_good/) : Great guide adressing input latency, audio latency and windows audio buffer latency
+ [How to make a practice difficulty efficiently](https://youtu.be/65nsCTLsTzk)
## Map packs
+ [ThePoon's 2020 osu! songs folder (55Gb)](https://www.reddit.com/r/osugame/comments/bfblao/updated_my_beatmaps_pack_torrent_55gb_many/)
+ [kwk alt map collection](https://docs.google.com/spreadsheets/d/14_lOp6k7CtGDAvJZ-ptYmSgO56sAhiqAqUZ_s5StbnU/edit?usp=sharing)
+ [Stream collection 2.0](https://www.reddit.com/r/osugame/comments/k3uwg8/stream_collection_20_is_here_120_300_bpm_1300/)
+ [Dragonforce maps list](https://docs.google.com/spreadsheets/d/1yO3QIGt50pT1BtCgZ50sqAIOirEcF0IApC3i13a4ScE/edit#gid=0)
+ [bog's speed map archive](https://docs.google.com/spreadsheets/d/14BDzlKmRXEnCNM65YKTE-J8TepRtIRAXMgDxKr9PdqQ/edit#gid=0)
+ [-Element-'s speed up packs](https://osu.ppy.sh/users/6113284) : check the user's "me!" section ;)


## Skins and skinning
+ [reddit community for skinning](https://www.reddit.com/r/osuskins/)
+ [osu!skins](https://skins.osuck.net/) : Huge skin archive (1500+ skins)
+ [osuskinner](https://osuskinner.com/) : Online skin maker
+ [Skin editor](https://osu.ppy.sh/community/forums/topics/486941?n=1) : Application to create/edit skins easily
+ [beatmapr](http://www.beatmapr.com/#/) : Online skin maker
+ [Circle people skins archive](https://circle-people.com/skins/) : Another skin archive
