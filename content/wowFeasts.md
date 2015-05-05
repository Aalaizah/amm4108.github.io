Title: Feasts in WoW
Date: 2015-05-03 19:58
Category: Development
Tags: HFOSS, BizLeg

Recently I realized that how I check what food or drink doesn't allow for eating a feast to affect your blood sugar level. 

#### Bag and Spell Casting
Currently, in order to figure out what food or drink you're consuming, it waits for your character to cast a spell. This sounds sort of weird, but in the back end, eating something in your bag is equivalent to casting a spell. The other thing it waits for is for something to update in your bag. If the spell that was cast is either a food or a drink then the bag update becomes important. 

When a food or drink spell is cast and the game registers that the contents of your bag changes, the add-on then checks to see what's different in your bags. It then takes that information and checks it against the list of food and drink items. 

#### Feasts Break it All
This set of checks works for almost all of the food types, however for raiding there are feasts. When you start eating from a feast it doesn't change anything in your bags. Because of this, there's nothing for the add-on to use to check against my list of foods. 

Feasts throw a huge wrench into the way the add-on works. Now that I have everything working and I'm just checking to make sure that my food list is correct, adding new functionality to check for feasts is next up.