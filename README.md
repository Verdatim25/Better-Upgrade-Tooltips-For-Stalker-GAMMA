# Better-Upgrade-Tooltips-For-Stalker-GAMMA
Better Upgrade Tooltips For Stalker GAMMA.

Showcase: https://youtu.be/x42r57RydZQ

# FOR GAMMA ONLY
I will not be providing support outside of gamma.

# Description
Changes the tool tip of upgrades to be accurate to the stat changes shown AND shows hidden stat changes. Also allows configuration of positive and negative upgrade stats.

## Explanation Of Stats
Weapon Stats:  
Accuracy -- Shows percent change of 'accuracy' stat.  
Handling -- Shows percent change of 'handling' stat.  
Recoil Control -- Shows change of the 'recoil control' stat. SEE NOTES BELOW.  
Reliability -- Shows percent change of the 'reliability' stat.  
Muzzle Velocity -- Shows velocity change of the 'Muzzle Velocity' stat (in m/s).  
RPM -- Shows RPM change of the 'RPM' stat (in RPM, rounds per minute).  
Weight -- Show weight change of the 'weight' stat of the item (in kg).  
  
Outfit Stats:  
Electrical Res -- Shows percent change of 'Electrical Res' stat.  
Burn Res -- Shows percent change of 'Burn Res' stat. SEE NOTES BELOW.  
Chemical Res -- Shows percent change of 'Chemical Res' stat.  
Psychic Res -- Shows percent change of 'Psy Res' stat.  
Rupture Res -- Shows percent change of 'Rupture Res' stat.  
Wound Healing -- Shows change of 'Wound Healing' stat, the unit is measure in (ml/min), making it equivalent to other sources of wound healing, like bandages.  
Health Restoration -- Shows  change of 'Health Restoration' stat. The unit is in line with regular artefact protection, so 1.5 health restoration is equivalent to 1.5 artefact health restoration (as shown in the artefact stat card).  
Radiation Res -- Shows percent change of 'Radiation Res' stat.  
Ballistic Res -- Shows change of 'Ballistic Res' stat.  
Stamina Recovery -- Shows change of 'Stamina Recovery' stat. The unit is (microgram of adren). This makes it equivalent to booster stamina recovery stats. So 80 microgram of adren for an upgrade is equivalent to that of the stamina recovery of a regular glucose shot.  
Condition Loss -- Shows percent change of 'Condition Loss' stat. In base GAMMA, each durability upgrade decreases the condition loss by 10%, so these upgrades are always labelled as "Condition Loss -10%".  

## MCM
In the MCM you can change what the text colour for the upgrade is, and optionally, you can change the negative upgrade text colour as well. By default, both settings are on and positive is green while negative is red.

# NOTES
## Rounding Errors
The script rounds up the number to 1 decimal place, meaning sometimes the stat can be off by 0.1.  
## RECOIL CONTROL:  
Recoil Control as a stat in game is weird. The formula for finding it boils down to 1/zoom_cam_dispersion * some_constant. This formula, unlike pretty much every other stat, is not linear. So the change of the recoil stat actually depends on the current value of the recoil stat. i.e. The differentiation is not a constant.  
In practice, this means the upgrade tool tip will show *different values* depending on how many upgrades you have on. THIS IS NOT A BUG, JUST A WEIRD QUIRK WITH HOW THE STAT IS CALCULATED, THE RECOIL CONTROL YOU GAIN IS ACCURATE.  
## BURN RES:
Burn Res in GAMMA 0.9.5 is broken in the stat card for outfits and helmets. It will show properly in the inventory defence section at the bottom but not on the stat card. DO NOT TELL ME ABOUT BURN RES NOT APPLYING PROPERLY. IT IS: ITS JUST NOT SHOWING IN THE OUTFIT STAT CARD.  

