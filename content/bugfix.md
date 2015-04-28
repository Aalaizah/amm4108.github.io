Title: Bug Fix
Date: 2015-2-24 02:26
Category: Development
Tags: HFOSS

### Finding It
While using an add-on that helps to track raiding achievements in World of Warcraft(WoW), I noticed that it was outputting some data wrong. When creating an add-on for WoW you can create what are called slash commands. These are commands that interact with your add-on specifically when a user types '/' and then the command. I noticed that instead of telling you to type '/achr' it was saying to type '/rach'.

### Reproducing It
1. Log in to WoW.
2. Open your add-ons list and ensure AchievementsReminder is turned on.
3. Enter any dungeon or raid instance that you can still earn ten or more achievements in.
4. Read the output and notice the incorrect slash command.

### Fixing It
Reading through other peoples add-on code is always interesting. You get to see the ways they decided to use what little Blizzard allows players to interact with in the in-game application program interface(API). A lot of add-ons use seperate files to save all of the text that will be output to the user. This allows you to easily implement localization. Looking through the english localization, I was able to quickly locate which variable was outputting the incorrect string and was able to correct it. From there I was able to do the same for most of the other localization files. Some of them, however, were done using a foreign alphabet, which made it so I wasn't able to correct those. 