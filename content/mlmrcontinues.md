Title: Master Loot Manager Remix 2.0 Continues
Date: 2015-2-16 23:45
Category: Development
Tags: BizLeg, HFOSS

This weekend was extremely productive towards Master Loot Manager Remix 2.0(MLMR2). I fixed a bug that came about from my earlier fix dealing with crossrealm raiding. I also added in a couple of different features that will hopefully help keep some drama out of the master loot process. 

The first deals with the idea that people can now kill a boss multiple times in one week, however they're only allowed to get loot the first time. This issue causes less drama, however it can still cause some. In order to combat this, I added a check before a character's roll is even reported in the add-on. If this check returns that you are eligible for the loot, the roll gets added to the list. Otherwise the addd-on just ignores it.

The other deals specifically with the characters chosen class and what armor category is optimum for them. For some classes, like the warrior, they can wear any type of armor, however wearing armor made of cloth won't give them as much protection as something made of plate. This next feature, just like the last, makes a check before the list updates with a characters roll. If the character either can't wear the armor or shouldn't wear the armor it won't show up in the roll list. 

In the future I would like to add another feature that prints out to the group why their roll wasn't added to the list. So far the reasons to be excluded include: rolling more than once(only first roll is included), not being eligible for loot from that specific boss, or it not being the optimum category for your class. This feature will also help deal with drama when people try to complain that you aren't reading their rolls, or that they had a higher roll, when really it was a second or maybe even third roll.