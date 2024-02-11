# Main Plot Plus
A plugin for the video game "endless sky" mostly centered around improving the main plot.

## Guided Start
This is an optional feature that can be enabled or disabled upon creating a new save or loading an existing one with this plugin installed for the first time. If you haven't chosen sides in the human civil war by 3017, Guided Start will allow you to join the Free Worlds, and also the Syndicate if you have the Crisis in Management plugin installed. It will additionally allow you to remain neutral (see below). Any conditions blocking the campaigns from starting will be cleared. If you depart and land or reload your save, then enter the spaceport, a map indicator will lead you to the planet to get started and remind you to enter the spaceport if necessary. This is necessary because the game only checks `to offer` conditions when landing or loading a save.

## Neutrality
You can choose to remain neutral in the human civil war. To do this, wait until 3023 without choosing sides, then when asked what side you are on, say that you are neutral. When pressed, continue to remain neutral. Shortly after, land on any world one jump away from a Pug planet and tell the Pug that you are neutral, and you will be able to skip the main plot. However, there's a catch: a different pilot will do the free worlds campaign instead, and they will choose checkmate. If you want the reconciliation ending, join the Syndicate with the Crisis in Management plugin or join the Free Worlds and choose reconciliation. The missions are designed so that you will be relocated to Ruin and time will advance by several years, but this is waiting on several pull requests to be merged, so at the moment you will have to use your imagination.

### Compatibility
Neutrality should be compatible with most major missions in the base game. You are told about the Pug war, the Free Worlds having nuclear weapons, and some of the new outfits produced by humanity: the plasma turret, flamethrower, s-970 regenerator, s-270 regenerator, ionic afterburner, typhoon torpedo launcher, electron beam, and catalytic ramscoop. This isn't everything, as it excludes the stack core due to it not being sold by Kraz Cybernetics, but it is enough to cover everything in the Coalition intros. You also learn about the Oathkeepers, and you assist Danforth by taking out a pirate fleet, unlocking the Wanderers campaign. From there, you can start Hai Reveal through Fiona and Rain, as the pirate fleet happened to have Hai weapons. I have additionally patched a mission that assumes you know Alondo. While Road to Hai Reveal only exists for Neutrality, I am planning on having a modified 'Road to Hai Reveal' for Crisis in Management after 1.0.0.

## Road to Hai Reveal
Hai Reveal is still in a work in progress state. Additionally, it at the moment requires you to specifically join the Free Worlds, or none of the missions after the leak will offer. As a result, I have a series of missions called "Road to Hai Reveal" that will allow you to do the intro of Hai Reveal if you have done Neutrality. I have also patched all the post-war reactions, see below. I have set it up so that you meet Alondo, which should allow the rest of Hai Reveal to work without issue if it gets merged as-is. If it gets changed to be more campaign agnostic, that still works and you can go down the free worlds path.

### Post War Reactions
The post-war reactions by default all assume you have directly fought with the Pug, which isn't necessarily true in Crisis in Management and definitely isn't true in the Neutrality option. I have replaced all three of these with patch missions which vary depending on how you interacted with the Pug, based on this plugin, the vanilla Free Worlds Reconciliation branch, and Crisis in Management. It also tries to test if you have done the vanilla version of Free Worlds Checkmate instead, if needed. I also removed a stupid section about the Free Worlds and Navy captains joking about almost killing each other. Other than that, doing Free Worlds should result in the same post-war reactions as vanilla, but doing Crisis in Management or the Neutrality option will give you different outcomes that make sense for what you've done.

## Syndicate
The Syndicate will now use their new technology on their ships if you complete the main plot, though they still won't sell it to you if you did reconciliation. The weights of the variants are based on the ones for the republic Mark II ships. A few of the Mark II variants are used in vanilla for a few missions in the reconciliation branch, but I added a bunch more so that all the Syndicate ships used in their main fleets have Mark II variants. The Syndicate rarely uses nuclear missiles before the war in the eastern parts of the Core, where they get raided by the Korath. They stop in 3014 because of the impending war.

### Test Dummies
Do you know those test dummy missions that you have to do? Well, there's a reason for them. Amazinite's Checkmate improvements include "automatic" ships. I have added these ships to occasionally show up in the Syndicate fleets after the main plot. They are essentially the same as the normal "mark II" ships, except that they have a special government that can change hails to use the test dummy ones, they cannot be bribed, they have the same confusion as the target practice jobs, they have the "automaton" and "self-destruct" attributes from the jobs, they are always called "Syndicate Test Vessel," and, being expensive, try to avoid battle and run away if threatened. Speaking of the test dummies, you can no longer fight them after the main plot, as the Syndicate has moved to the next phase of their testing and has started to incorporate them in their fleet.

## Improved Checkmate
Amazinite had, a long time ago, added changes that improved the Checkmate branch, that ultimately didn't go anywhere, other than some changes in the first part of the campaign rework. These changes will likely be added as part of the next parts of the campaign rework. However, as I am a fan of the Checkmate branch already, I think more people should be doing it, so I am incorporating these changes now, along with some minor fixes. Mostly, these allow you to ask about progress made by the Syndicate in finding the terrorists, and eventually allow you to "fight" them with automatic ships after the Pug invasion. I am also changing one major thing: the nuke launcher has been replaced with "augmented nuclear missiles," which are essentially the buffed nuclear missiles proposed by Azure3141. When these begin being sold, the Syndicate also begin using them instead of regular nukes in a new "Mark II Nuclear" loadout in the systems raided by the Korath. This Manta loadout has four augmented nuclear missiles and two sidewinder missile launchers, the latter of which ensures that the Mantas use the "missile boat" AI, making them less likely to blow themselves up. This updated plot is referenced in the Neutrality option, mentioning the Syndicate finding the "terrorists" and the automatic vessels being used as cannon fodder.

## Deep Science Drones
0.10.5 added the sunder and mining drones, so I decided that it was time to allow you to get your own science drones! Some time after you do project hawking, Valhalla and Asgard will begin selling a drone variant of the aerie along with science drones, and a fleets consisting of an aerie with two science drones will begin to travel around the Deep. A few months later, miners will begin using the drone variant with mining drones to mine. The aerie drone variant is also occasionally used by the pirate fleet in road to hai reveal.

## Bugs
I have playtested this plugin and fixed any bugs, edge cases, and warnings I could find. There may still be bugs, and bug reports and pull requests fixing bugs are welcome. This is currently in a beta release while I work on re-organization based on the structural guidelines and a machine-readable copyright file. Note that the beta release has known bugs that have been fixed upstream. Please be patient while I make final changes before releasing the plugin fully.

## Other Plugins
There is a plugin called "Constellations" that modifies the Pug wormhole to point to Queri instead of Over the Rainbow. As remaining neutral will eventually send you to Ruin once the relevant PR is merged, this change would softlock the game. As a result, remaining neutral will cause the wormhole to point to Over the Rainbow, as is the case in vanilla. I could have made it kick you out of the Pug galaxy permanently once you leave, but this seems like it would create more problems than it would solve, at least to me. If you don't like the decision I made, this plugin is open source. Just modify it.

As for Crisis in Management, my plugin takes it into account as much as possible, with the exception of Road to Hai Reveal. This means you still cannot do Hai Reveal if you did Crisis in Management, however, I will work on this after 1.0.0.

## Copyright
This plugin was initially dedicated to the public domain, however, I have taken and modified text from missions in the base game, which is technically code, so it is now licensed under the GPL v3 or later to ensure that I do not violate the endless sky license terms. See the "copyright" file for more details. I am working on a machine readable copyright file for the full release, which will be added to debian/copyright.

## Note on Breaking Changes
I have made one Beta release, which means that there will be no more "breaking" changes. For those who just downloaded the Beta release, I still make no guarantees, but I will try to prevent save issues from now on. Note that I still may rename missions, for instance, but I will provide patch missions, whereas before this wasn't the case. However, those playing before the release will likely have to go through breaking changes when updating to the Beta branch, including, but not limited to, renaming the plugin, renaming files, removing files, reorganizing files, splitting files, merging files, and modifying data files without providing patch missions or other backwards compatibility features. For those who tested out my plugin before release, thank you, but treat this like you would the "continuous" branch of Endless Sky, except for updates after the Beta release, and do not be surprised if you end up with broken saves. Remember, there is no warranty.

