Title: WoW Diabetes - Import/Export Issues
Date: 2015-3-19 17:34
Category: Development
Tags: HFOSS, BizLeg

#### It's All Borked!
I've been trying to add in the things I will need to be able to export stats to our website and then be able to import them back in if the player needs it. I've tried a few different ways of doing things, but most of them have ended in an error where something that should exist through the Blizzard UI doesn't exist. All of these errors made the game itself unplayable while my add-on was running, a couple of times the errors I was getting made it so I had to do a hard reload in order to reset the add-on.

#### I Think I fixed it!
After looking through not only some other add-ons but also some of Blizzard's UI code, I found something that seems to be working. There aren't any runtime/compiler errors, but I also haven't finished implementing everything. As I move in to spring break I will hopefully get the last of it implemented and running so that as soon as the website is fully functional we can go live with that update.