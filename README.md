# Dead_Simple_Sprite_Mod
Okay, I'll be upfront: I decided to call the mod this when it was ACTUALLY just a sprite replacement with minimal DeHackEd work - just intended to make the vanilla experience look and feel a little better.  As usual, once I started playing with DeHackEd I just couldn't stop, so now what I've ended up with is an MBF-compatible smooth (mostly) weapons mod with a few monster tweaks to go along with it.  I'm keeping the name, if only for the sense of irony it provides. My new goal became to make this mod "what KexDoom should have looked like", since **I was able to do ALL of this with the vanilla state table with zero states pulled from decorations**. I originally had it as Boom-compatible but I NEEDED one of the MBF pointers for something so c'est la vie, **it still runs in Crispy Doom**.  Weapon sprites have been adapted from Brutal Doom v22, the Vanilla Gloves mod for v21, Major Crisis, c0mbolynch's weapon reskin for SuperCharge, and Doom Forever. Nearly all of the pickup sprites have received at least minor reworks to both more closely resemble the sprites from the player's POV and also to look more like they could be actual weapons.  
I have meticulously gone frame-by-frame to make sure the timing on the weapons matches exactly with their equivalents in Vanilla.  That being said, I wouldn't recommend using this mod for demo recording or playback because every projectile for both player and enemy has gotten a speed buff, and one weapon and a couple enemies have been tweaked in such a way that may cause a desync, but the projectiles are definitely the bigger concern.  On a more positive note:
**No weird purple and red artifacts here; this mod is also 100% pallette-compatible with BTSX!**

**NEW WEAPON CHANGES:**
- The fist remains mechanically unchanged but uses a separate "pull" frame after punching to give a better impression of follow-through and pulling back.
- The chainsaw remains mechanically unchanged but I've halved the frame hold time on the Ready state to make the chain look like it's spinning more smoothly.
- The pistol no longer tries to jump out of your hand when trying to fire, and also looks more like actually shooting a handgun.
- The shotgun has been given double its original frames, and now ejects a shell casing.
- The Super Shotgun has been given TRIPLE its original frames, also ejects shell casings, 
- The Chaingun is now a submachine gun with all the same characteristics as the chaingun with the sole exception that it fires one bullet per pull of the trigger, rather than two.  Rate of fire remains unchanged.
- The Rocket Launcher has better sprites and a smooth animation, complete with rotating cylinder. ﻿
- The Plasma Rifle is smooth and no longer ugly as sin.
- The BFG is definitely the most questionable change here, but I still think it looks overall better than the original.

NEW ENEMY CHANGES:
- The Zombieman has been given fullbright on his firing frame and calls refire like the chaingunner whenever he still has line of sight of the player character.  He also has a new death animation.
- Lost Souls do not bleed.
- ShotgunGuy has been given a new death animation, a Spawn animation unique from the See sprites, and also visibly pumps his shotgun after each shot.
- Since the chaingun is now an SMG, the Chaingunner has been replaced by a Machinegunner I made, who will drop the SMG on death. His rate of fire remains unchanged from the original, but the frame duration has been halved to make the animation match the rate of fire.
- Imp pre-firing frames got a little hotter...
- Barons now have green blood in supported ports and black legs to make them a little easier to differentiate at a distance from Hell Knights.
- Cacodemons, Hell Knights, Barons, and Pain Elementals also haave blue, green, and orange blood, respectively, in supported ports.
- Revenants now wear black armor.  This has no in-game purpose, I just think it looks sick af.
- New sprites for the shocktrooper and their forcefully-separated head in Legacy of Rust
- New gorier death animation for the Archvile (deserved).

BRIGHTMAPS: 
WE GOT EM (in supported ports).  Enemies now have glowing eyes and cybernetic enemies also have glowing machine bits, in addition to flats for nukage and lava and most pickup sprites having something on them that glows, if appropriate.  Imps and bruisers also have glowing hands as they prepare to fire.

NUGHUD: Included a minimalist NUGHUD file for Nugget Doom users.

DEHEXTRA ADD-ON:
Hey man, y'all like smooth decorations and powerups?  Dead Simple now comes with a small DEHEXTRA-compatible add-on that can be loaded alongside the other included add-ons to get:
- Animated Medikits
- Smooth health potions
- Smooth torches and barrels
- Spinny keys and skulls
- A super cool trail effect for plasma balls
- Compatibility built-in with the brightmaps lump

Add it in your load order after the gameplay mod of your choosing today!! Or don't, I'm not your boss!

THIS MOD HAS BEEN TESTED AND IS FULLY* COMPATIBLE WITH:
- The Woof! family of ports (incuding Nugget and Cherry)
- Doom Retro
- DSDA-Doom
- Crispy Doom
- GZDoom
- The Eternity Engine 

*KNOWN ISSUES:
- Currently, of the ports I've tested here, only Woof!-family ports are able to accept the BRGHTMPS lump, though Doom Retro should be fixing this feature in an update following 5.7.1.  All of the Woof!-family ports would crash loading Legacy of Rust when I tested them with BRGHTMPS included in the WAD.  Removing it fixed the crash, and adding it separately in the load order let me have our brightmaps back.  To avoid including three different versions of the same WAD in this folder, I've opted to simply include the separate BRGHTMPS lump to load as you see fit.
- Doom Retro and GZDoom both like to CTD when you quit after playing BTSX, but at that point you've already quit so I'm honestly not _that_ worried about it.
- DSDA, Eternity Engine, and GZDoom have a REALLY choppy chainsaw bob.  It doesn't affect the performance and comparing it to vanilla, I think that may actually be the default behavior, but I figured I'd make a note of it regardless. 

HOW TO USE:
If your source port has an autoload folder and you want to use them, you can go ahead and add brghtmps.lmp and the NUGHUD into the "all" section and just skip anything related to them in the instructions below.  
Load order matters here, though in most instances it's no different than you're used to.  If you're NOT playing Legacy of Rust, load the IWAD, then map PWAD, then the weapons mod of your choosing, then brghtmps.lmp and the NUGHUD if you're playing with a Woof!-family port and so-desire.  If you ARE playing Legacy of Rust, the weapons mod must be loaded BEFORE Legacy of Rust to allow overwriting the Plasma Rifle and BFG.  The Rust Patch must be loaded afterwards to put the new shocktrooper sprites and strings consistent with the LoR content in the game.  Regardless the gameplay mod you're using, load DeadSimpleExtra.wad after the mod.  Brghtmps.lmp and the NUGHUD go at the end as per usual.

CREDITS:
- Sgt Mark IV - Brutal Doom v21 and v22 (Fist, Pistol, Shotgun, BFG)
- OSJC Latchford - Major Crisis (SMG, Plasma Rifle)
- Sonik.O.Fan aka Tesefy - Brutal Doom v21 Vanilla Gloves (Rocket Launcher)
- Lobo - Doom Forever (Imp Sprites, some effects)
- c0mbolynch - Supercharge weapons addon (Super Shotgun)
