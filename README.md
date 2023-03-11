# Planet Jam 2 Alternate Realism Configuration

[Planet Jam 2: the Ilio-Pyri System](https://forum.kerbalspaceprogram.com/index.php?/topic/211156-v101-central-fire-planet-jam-2-armstrongs-limit-homeworld-in-the-ilio-pyri-planetary-system/) is a fantastic planet mod, full of variety, possibilities, and of course many, many interesting planets.
As a collaboration between 15 different authors, different parts of the system inevitably ended up with different styles that don't always quite match. This is perfectly fine, but I personally prefer a bit more internal consistency, and the easiest way to do that is by adding ~~realism~~.

Well, at least the KSP version of "realism". Everything might be ten times too dense compared to the real world, but at least it's exactly ten times too dense. It's consistent, which I believe is one reason why that one particular fact about the kerbal universe is so widely accepted.

PJ2ARC is a collection of Module Manager patches that make the planets more "kerbalistic" while attempting to preserve the original intentions of the authors. Many of the patches are optional, so you can choose which ones you want to apply and which you think are unhelpful or going too far.

### Enabled by default
#### Viszra density increase
* Increases Viszra's surface gravity to 0.2139 g. This is not necessary on its own but makes the following patch work much better, as it lowers Viszra's calculated atmosphere height from 196 km to 151 km and raises its SOI altitude from 201 km to 288 km.
#### Oynag system atmospheres
* Expands the atmospheres of Viszra, Jejunum, Cricoid, and Zeppeli outwards to realistic scale heights.
* Viszra's atmosphere now ends at 151 km, Jejunum's at 86 km, Cricoid's at 147 km, and Zeppeli's at 91 km.
##### Scatterer integration
* Raises the Scatterer scale heights to match the new Oynag system atmospheres. Does nothing if the Oynag patch is disabled.
#### Bugfixes
These patches fix what I consider to be true internal consistency issues.
##### Ilmar oxygen
* Adds oxygen to Ilmar's atmosphere to match its description in the Tracking Station.
##### Jones temperature
* Raises Jones's atmospheric temperature to 100 K to match the value in the Tracking Station.

#### Tobalk atmosphere
Adds a thin hydrogen-nitrogen-helium atmosphere to Tobalk. (I assume that it was originally hydrogen-dominated but lost almost all of its hydrogen and most of its helium to Turtlestar.)
* 25 km total height, which is below the highest terrain and so will not affect stable orbits.
* 3 atm at the datum level. This is actually quite dense, but Tobalk's high gravity means that the atmosphere thins out extremely quickly and is practically negligible above 10 km, where most of the terrain is. At orbital velocities, however, it can be significant as long as you don't run into a mountain.
* Integration with Scatterer. Much of the scattering is not actually visible, but it does change how Tobalk appears when eclipsed by Turtlestar.


### Disabled by default

#### Selectable spoilers
* Allows you to find [REDACTED] again by clicking [REDACTED] in the [REDACTED].

(This is intentionally vague because it's a big spoiler. If you don't know what it means, don't apply the patch because that could spoil it.)

### Enabled automatically
#### Previous features
PJ2ARC used to have an entirely different set of changes, which were then integrated into PJ2. That version of PJ2 has not yet been released, so those changes have been kept here and revised to match their PJ2 implementation.
#### Beddul albedo revision
* I had incorrectly assumed an albedo of 0.1 for Beddul. This has been revised to 0.4, lowering the height of its atmosphere to 68 km.


### Delta-v table
A [delta-v table](https://docs.google.com/spreadsheets/d/1891mTQLAGPMRzXrHoydCgmZXNDeHMkVCEddytleJYnE/edit?usp=sharing) is available, including all the changes to celestial body masses and orbit altitudes. For comparison, a table for PJ2 1.0.1 with no changes is available [here](https://docs.google.com/spreadsheets/d/1viA1pa6PS0U2Wi2cbCBXtvaUrr9k0LIK65WDvR5vL3U/edit?usp=sharing).
