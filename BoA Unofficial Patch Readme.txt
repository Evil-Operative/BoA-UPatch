=========================================
Blades of Avernum Unofficial Patch v1.0.0
   Created by Sokhbep and friends :D
=========================================

Please contact me (Sokhbep) on the Spiderweb Forums or @Ecl1p5e#8061 (also me) on Discord if any errors or shortcomings are discovered! I am also usually found on the Official Spiderweb Software Discord Server. - https://discord.com/invite/fAHCRYQ

o------------------------------------------------------------------------------o
| Credits to: Ishad Nha - Compiling bugs                                       |
|	      Kelandon  - Custom Objects Script Base (COSB) and Compiling bugs |
o------------------------------------------------------------------------------o

============
INSTRUCTIONS
============

BEFORE DOING ANYTHING, PLEASE BACKUP YOUR "Data" FOLDER ELSEWHERE ON YOUR COMPUTER AS A COPY. IT IS A SOUND ADVICE IF YOU DO NOT WISH TO DOWNLOAD AND INSTALL THE GAME AGAIN TO RESTORE YOUR FILES BACK TO NORMAL!!

(1) The .zip file comes with two components - 'BoA UPatch 1.0.0.exe' and a "Data" folder consisting of the rest of the modified files.

'BoA UPatch 1.0.0.exe' is a companion executable file which is supposed to be opened instead of the normal 'Blades of Avernum.exe' in order to change a few internal things which cannot be achieved by modifying the game scripts or graphics.

The "Data" folder mostly contains everything ready to replace the stuff in your Blades of Avernum folder, which includes the edited graphics files. But there are two things which need your manual attention. For that, please follow Step 2.

- To patch the executable file, simply drop it into your "Blades of Avernum" folder. It does not need to replace/overwrite the default executable file to work.
- To patch the "Data" folder, simply copy and paste it into your Blades of Avernum folder and let it replace/overwrite all the files. Once it is done, open the folder and follow the steps below.


(2) In the Data folder included within the .zip file (the one you have just copied and pasted over into your Blades of Avernum folder), there are two variants of 'corescendata' and 'corescendata2':

- The 'coloradjust' variant makes various flavourful colour changes to some items and creatures using the 'icon_adjust' function to make them different in looks from each other along with the necessary patches and fixes listed below. 
- The 'nocoloradjust' variant skips the "flavourful recolouring" part entirely and only carries the patches and fixes. This alternative is for those who do not care about my rainbows and glitter and want only the part that means business.

Once you have figured out which variant of the patch you wish to apply, delete the previous (unpatched) versions of 'corescendata.txt' and 'corescendata2.txt' that already exist in your 'Data' folder, then whichever variant of the patch you wish to apply, simply rename both parts of it such as, for example: 'corescendata_nocoloradjust.txt' --> 'corescendata.txt'.

(Note: You are completely free to edit the scripts to your liking. I understand that not everybody is going to unanimously agree on all of my changes, and therefore the files are all there for you to selectively modify or exclude from the patching process. After all, who am I to judge the people who'd rather have their Ruby Skeletons appear outdoors with their older artwork? Just don't replace 'G1581.bmp' and you're all set.)


[OPTIONAL STEP] Similarly there are modified graphics for G812, G813 and G816 with the '_edited' suffix which add a few flavourful changes on top of the patches listed in the changelog. These changes alter the look of some spells and abilities such as giving 'Arcane Blow' spell icon a purple fill instead of the old cyan one based on how the spell looks when used on enemies, and restoring the old 'Summon Beast' ability icon from Avernum 1-3.

===================================
CHANGELOG v1.0.0 - 05 December 2021
===================================

///[ BoA UPatch.exe ]\\\ (You must run the game through this file in order to experiences these changes)

-  The hand icon in the Get Item dialog box is now a right-handed cursor instead of being a left-handed one. Since all the other cursors in the game are right-handed, it doesn't make much sense to keep just one cursor left-handed


///[ corescendata.txt ]\\\

Floors 85 and 86 'Crops' icons are no longer erroneously swapped
Floor 100 'Vahnatai Floor' now has a correctly coloured editor icon [COSB]
Fixed capitalisation errors on the second words of many creature names (e.g. Lava bat, Triad mage, Slith high priest etc.)
Creatures 71 'Aranea' and 83 'Elder Aranea' now have 'Pots' removed from their respective death drop tables
Creature 100 'Slith Avatar' now has the correct icon adjust colour of 2 instead of 64 [COSB]
Creature 135 'Augmented Giant' now correctly displays its upper half [COSB]
Creature 174 'Efreet' no longer has duplicate natural armor value '15'. It now only has '50' natural armor


///[ corescendata2.txt ]\\\

Terrains 331 and 332 'Cave Hill Entrance' now correctly import the proper direction of the terrain 'Cave Hill' so that players standing on the same tile do not have their placement look messed up
Terrain 367 'Ruined Statue' has its upper half restored
Terrain 396 'Supply Cache' has the Terrain 397 'Found Supply Cache' as its terrain swap [COSB]
Item 74 'Cursed Halberd' is now properly cursed. It had the cursed property defined twice, the second time un-cursing the item
Item 166 'Jug of Cheap Wine' renamed to 'Jug of Cheap Ale', Item 393 'Cheap Wine' renamed to 'Jug of Cheap Wine' and value increased from 20 coins to 45 coins. Changed to make a redundant item have more flavourful correlation with pre-existing items 'Bottle of Ale and 'Bottle of Wine' respectively
Item 149 'Bowl' now uses the correct floor graphic
Item 154 'Bolt of Cloth' now uses the dark green alternate variant whose floor icon has been restored and thus now looks different from Item 156
Item 345 'Icy Longsword' now correctly inflicts extra cold damage instead of extra acid damage
Item 369 'Wyrmsbane' buffed - now imports from 'Blessed Longsword' instead of 'Bronze Longsword' and has its value increased from 40 coins to 2400 coins 
(Like for real, come on.. this epic sword that does more damage to snakes, lizards, drakes and DRAGONS used to inherit from a weak weapon and was almost worthless. Also I'm 99.9% sure the wrong import was used in the first place, since 'Ghoulbane' inherits from 'Blessed Spear' and does the same amount of damage bonus but to undead)
Item 432 'Ring of Speed' buffed - now has a chance of giving a maximum of 2 bonus AP instead of 1, which is already emulated by Item 277 'Nimble Band', thus making the former an upgraded version of the latter instead of being completely same

Changed 'Wand', 'Crystal' and 'Rod' items to have the same naming scheme as Scrolls e.g. "Wand - Bolt of Fire", "Crystal - Dispel Barrier"
Fixed some items not graphically representing their class e.g. 'Cursed Short Sword' used a 'Longsword' graphic and 'Jade Halberd' used a 'Spear' graphic
Swapped around 'Ring' item graphics to distribute each type of graphic among the items equally. Each ring graphic type now has at least one cursed variety
Rearranged all 'Scroll' item graphics so that one particular graphic type represents only one of the four separate spell types: direct damage, support, utility and summon
Rearranged all 'Wand' item graphics so that one particular graphic type represents only one of the three separate spell types: direct damage, support and utility
Changed some item names in order to maintain uniformity with similar item types (e.g. renamed 'Blessed Steel Helmet' to 'Blessed Helmet', changed the unidentified name of 'Alien Blade' from 'Wavy Sword' to 'Waveblade')

Readjusted the graphics of entirety of the artifact shield lineup based on the following statistics:

0% Encumbrance, uses the artifact light shield graphic (G1035 - Out 4 - In 5)
- Runeshield

5% Encumbrance, uses the artifact medium shield graphic (G1035 - Out 0 - In 1)
- Crystal Shield
- Iceshield
- Shield of Khar
- Shield of Klin

10% Encumbrance, uses the artifact heavy shield graphic (G1030 - Out 0 - In 1)
- Shield of Klud
- Shield of Kron
- Martyr's Shield
- Lifeshield


///[ Character Graphics ]\\\

Fixed missing border pieces for the following files: 
G1452 (Kobold)
G1554 (Lizard)
G1562 (Vampire)
G1564 (Granite Golem)
G1565 (Triad Mage)
G1569 (Erika)
G1570 (Demon Lord)
G1574 (Royal Guard)
G1587 (Vahnatai w/ Green Cloak)

Other graphical changes were made in the following files:
G1 (Empty Space) - Fixed image dimensions
G1453 (Centaur) - Removed protrusions on outdoor graphic
G1500 & G1501 (Merchant w/ Blue Pants) - Fixed erroneous white/transparent pixels on various frames
G1524 (Nephil Archer) - Removed protrusions on outdoor graphic
G1533 (Slime Pool) - Added outdoor graphics
G1535 (Skeleton) - Removed protrusions on outdoor graphic
G1537 (Ghoul) - Fixed erroneous white/transparent pixels on various frames
G1539 (Wight) - Fixed black outlines on death frames
G1542 (Giant Lizard) - Fixed erroneous white/transparent pixels on various frames
G1543 (Fire Lizard) - Fixed erroneous white/transparent pixels on various frames, and erroneous outlines on death frames
G1547 (Drake) - Fixed black outlines on death frames
G1549 (Demon) - Fixed erroneous white/transparent pixels on various frames and fixed missing border piece
G1550 (Haakai) - Fixed erroneous white/transparent pixels on various frames
G1551 (Serpent) - Fixed incorrect facing directions on North and West
G1552 (Eye Beast) - Fixed incorrect facing directions on North, West, South and East
G1553 (Living Statue) - Fixed erroneous white/transparent pixels on various frames and fixed incorrect outdoor graphics (Gremlin)
G1561 (Child) - Added outdoor graphics
G1566 (Gorgon) - Fixed erroneous white/transparent pixels on various frames
G1568 (Spider Queen) - Adjusted outdoor sprite colours to match indoor sprites
G1571 (Pack Leader) - Fixed erroneous white/transparent pixels on various frames
G1575 (Townsman w/ Black Vest) - Fixed erroneous white/transparent pixels on various frames
G1577 (Bladesman) - Removed protrusions on outdoor graphic
G1581 (Ruby Skeleton) - Updated outdoor graphics to new sprites, was previously using old A1-3 Ruby Skeleton sprites 
G1582 (Spectre) - Removed protrusions on outdoor graphic and fixed erroneous white/transparent pixels on various frames
G1583 (Hraithe) - Removed protrusions on outdoor graphic and stray pixels outside the frames window
G1584 (Vahnavoi) - Fixed stray pixels outside the frames window
G1585 (Ice Lizard) - Fixed erroneous white/transparent pixels, off-black border colour and coloured pixels on various frames
G1588 (Vahnatai w/ Yellow Cloak) - Fixed erroneous white/transparent pixels on various frames
G1589 (Vahnatai Child) - Added outdoor graphics and removed stray pixels outside the frames window
G1596 (Crystal Soul) - Added outdoor graphics
G1597 (Doomguard) - Removed protrusions on outdoor graphic
G1600 (Hydra) - Fixed incorrect outdoor graphics (Baby Hydra)
G1601 (Flame Hydra) - Fixed off-black border colour
G1602 (Ice Hydra) - Fixed off-black border colour
G1603 (Baby Hydra) - Fixed erroneous white/transparent pixels on various frames
G1604 (Ice Drake) - Fixed black outlines on death frames
G1607 (Rakshasa) - Improved outdoor graphics
G1608 (Naga Bottom) - Improved outdoor graphics and moved incorrectly placed outdoor graphics on top half of sheet to bottom half
G1609 (Naga Top) - Removed redundant outdoor graphics
G1615 (Giant Fighter Bottom) - Updated outdoor graphics to new sprites, was previously using old A2-3 Giant Fighter sprites
G1616 (Giant Fighter Top) - Removed redundant outdoor graphics
G1617 (Giant Chief Bottom) - Updated outdoor graphics to new sprites, was previously using old A2-3 Giant Fighter sprites
G1618 (Giant Chief Top) - Fixed erroneous white/transparent pixels on various frames
G1619 (Dragon Bottom) - Moved incorrectly placed outdoor graphics on top half of sheet to bottom half
G1620 (Dragon Top) - Removed redundant outdoor graphics
G1621 (Efreet) - Updated outdoor graphics to new sprites, was previously using old A2-3 Giant Fighter sprites
G1627 (Wolf) - Fixed erroneous white/transparent pixels on various frames
G1628 (Worg) - Fixed stray pixels outside the frames window
G1630 (Amber Slime) - Fixed South facing outdoor sprite being smaller in scale than the rest
G1631 (Ochre Slime) - Updated North and West outdoor graphics to actually face North and West
G1633 (Mauve Slime) - Removed protrusions on outdoor graphic
G1634 (Royal Slime) - Fixed erroneous white/transparent pixels and added outdoor graphics
G1637 (Large Roach) - Fixed incorrect facing directions on outdoor graphics. South and East were earlier facing North and West respectively
G1649 (Mind Crystal) - Removed protrusions on outdoor graphic


///[ Art Graphics ]\\\

G1650 (Red-haired Man) - Updated armored outdoors sprites to match armored indoor sprites
G1651 (Barbarian Man) - Updated armored outdoors sprites to match armored indoor sprites
G1652 (Barbarian Woman) - Updated armored outdoors sprites to match armored indoor sprites
G1653 (Purple Garb Man) - Updated armored outdoors sprites to match armored indoor sprites
G1654 (Bow on Back Woman) - Fixed armored pole sprites not actually having armor, armored sword/shield sprites not having either shield or armor and updated armored outdoors sprites to match armored indoor sprites
G1655 (Blue Cape Man) - Updated armored outdoors sprites to match armored indoor sprites
G1660 (Brown Vest Bandana Man) - Updated armored outdoors sprites to match armored indoor sprites
G1663 (Green Sorceress Woman) - Updated armored outdoors sprites to match armored indoor sprites
G1666 (Brown Vest Apron Man) - Updated armored outdoors sprites to match armored indoor sprites
G1666 (Brown Vest Apron Woman) - Updated unarmored outdoors sprites to match unarmored indoor sprites (combo breaker!!)
G1668 (Red Armor Nephil) - Updated armored outdoors sprites to match armored indoor sprites
G1669 (Pink Armor Nephil) - Updated armored outdoors sprites to match armored indoor sprites
G1670 (Golden Fur Nephil) - Updated armored outdoors sprites to match armored indoor sprites
G1671 (Blue Armor Light Nephil) - Updated armored outdoors sprites to match armored indoor sprites
G1672 (Blue Armor Dark Nephil) - Updated armored outdoors sprites to match armored indoor sprites
G1673 (Orange Frilled Dark Slith) - Updated armored outdoors sprites to match armored indoor sprites
G1674 (Gold Frilled Slith) - Updated armored outdoors sprites to match armored indoor sprites
G1675 (Orange Frilled Light Slith) - Updated armored outdoors sprites to match armored indoor sprites
G1676 (Brown Frilled Slith) - Updated armored outdoors sprites to match armored indoor sprites
G1677 (Pink Hooded Slith) - Updated armored outdoors sprites to match armored indoor sprites and fixed erroneous white/transparent pixels on various frames
G1680 (PCs on Horseback Indoors) - Changed every direction sprite to be armored instead of just some directions and fixed missing border piece
G1681 (PCs on Horseback Outdoors) - Changed every direction sprite to be armored instead of just some directions and fixed stray pixels outside the frames window


///[ Game Graphics ]\\\

G812 (Mage Spells Icons) - Fixed 'Capture Mind' icon erratic x-offset
G813 (Priest Spells Icons) - Removed stray graphic bits outside of the displayed area
G814 (Make Potion Icons) - Swapped Strength Elixir and Rogue's Elixir graphics to maintain uniformity (Rogue's Elixir used to use the brighter version of the Strength Potion icon)


///[ Item Graphics ]\\\

Fixed erroneous white/transparent pixels on the following graphics:
G1000	G1004	G1004
G1020	G1029	G1037
G1048

G1005 - Touched up 'Cudgel' floor graphic to match inventory graphic
G1010 - Restored dropped item graphic for the dark green variant of 'Bolt of Cloth'
G1029 - Touched up 'Iron Greaves' graphics to not have fuzzy white pixels 
G1032 - Changed 'Basket' floor graphic to match inventory graphic
G1033 - Touched up 'Sling' floor graphic, edited 'Towel' floor graphic to match inventory graphic
G1045 - Changed the second 'Scroll' icon's floor graphic to match inventory graphic and flipped the first 'Scroll' icon's floor graphic
G1046 - Changed 'Crude Short Sword', 'Steel Short Sword', 'Scimitar' and 'Greatsword' floor graphics to match their respective inventory graphics
Fixed missing border pieces for pretty much every single file in the folder


///[ Terrain Graphics ]\\\

Fixed erroneous white/transparent pixels on the following graphics:
G618	G702	G703
G704	G720	G724	
G725	G768	G796

G680, Icon 52 flipped horizontally to match the in-game graphic
Fixed missing border pieces for pretty much every single file in the folder
