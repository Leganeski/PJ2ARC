# Planet Jam 2 Alternate Realism Configuration

[Planet Jam 2: the Ilio-Pyri System](https://forum.kerbalspaceprogram.com/index.php?/topic/211156-v101-central-fire-planet-jam-2-armstrongs-limit-homeworld-in-the-ilio-pyri-planetary-system/) is a fantastic planet mod, full of variety, possibilities, and of course many, many interesting planets.
As a collaboration between 15 different authors, different parts of the system inevitably ended up with different styles that don't always quite match. This is perfectly fine, but I personally prefer a bit more internal consistency, and the easiest way to do that is by adding ~~realism~~.

Well, at least the KSP version of "realism". Everything might be ten times too dense compared to the real world, but at least it's exactly ten times too dense. It's consistent, which I believe is one reason why that one particular fact about the kerbal universe is so widely accepted.

PJ2ARC is a collection of Module Manager patches that make the planets more "kerbalistic" while trying my best to preserve the original intentions of the authors. Everything is customizable, so you can choose which patches you want to apply and which you think are unhelpful or going too far.

The options are as follows:

### Enabled by default
#### Ollo density patch
Each body in the Ollo system has an explanation describing how its mass is the product of its density and its volume, whis fails to consider the increased density of kerbal-scale objects. The volumes are correct, so the masses must be increased by a factor 10 to make the densities more realistic. The relative masses and SOIs remain unchanged, while orbital periods are decreased by sqrt(10).

#### Asteroid density patch 
Miscellaneous changes to densities of very small moons.

* Phe mass x100 (new (kerbal-scale) density 3.16 g/cm<sup>3</sup>)
* Ber mass x100 (new density 3.73 g/cm<sup>3</sup>)
* Phomos mass x160, or uses geeASL instead of mass if available (new density 4.18 g/cm<sup>3</sup>)
* Rangon mass x100 (new density 11.65 g/cm<sup>3</sup>)
* Blitzø mass x0.1 (new density 2.17 g/cm<sup>3</sup>)
  
#### Ocean density patch
Jejunum's ocean has a comment describing it to be methane, but liquid methane would boil away in the conditions at the bottom of the atmosphere. The ocean's scorching temperature and orange color demonstrate that it is actually lava instead, so its density is increased to 3.1 g/cm<sup>3</sup>.

#### Oynag system atmosphere fix
Every atmosphere in the Oynag-Descry system has the default molar mass of 2.2 g/mol, indicating a composition of mostly hydrogen. This is appropriate for the giants, but molecular hydrogen on any of the solid moons would quickly escape into space. The most likely primary constituent of these atmospheres is nitrogen, which has a molar mass of 28 g/mol.
* Viszra atmosphere molar mass increased to 27.41 g/mol (95% nitrogen, 5% methane)
* Jejunum atmosphere molar mass increased to 28.01 g/mol (100% nitrogen)
* Cricoid atmosphere molar mass increased to 28.01 g/mol (100% nitrogen)
* Zeppeli atmosphere molar mass increased to 28.05 g/mol (98% nitrogen, 2% methane)

#### Beddul-Dopale atmosphere overhaul
Beddul and Dopale have atmospheres that are perfectly understandable at the surface, but thin out unusually slowly before suddenly ending. These would be fine on their own, but are somewhat out of place in a star system with so many other atmospheres that thin out more gradually.

All atmosphere curves (temperature-latitude, temperature-altitude, pressure-altitude) have been replaced with new ones from OhioBob's [realistic atmosphere calculator](https://forum.kerbalspaceprogram.com/index.php?/topic/158163-make-your-own-atmospheres-for-ksp-automatically/).
Carbon dioxide alone can't account for Beddul's high temperature, so near the surface, the temperature-altitude curve transitions from the calculator-generated curve to the given surface temperature of 566 K.

* Beddul's atmosphere is assumed to be 73.5% CO<sub>2</sub>, 25.5% N<sub>2</sub>, and 1% H<sub>2</sub>O. Its height is reduced to 73 km.
* Dopale's atmosphere is assumed to be 93.1% N<sub>2</sub>, 6.8% CO<sub>2</sub>, and 0.1% H<sub>2</sub>O. Its height is reduced to 63 km.

### Disabled by default

#### Jones overhaul
Jones needs to have its density decreased by 10. However, there are a number of factors making this complicated, especially its atmosphere.
* Radius increased by x10; mass increased x100. (New density 1.12 g/cm<sup>3</sup>.)
* Surface gravity unchanged.
* SOI increases to 127.078 km, or 35.878 km above the datum level.
* Surface atmospheric conditions unchanged. The unusually cold temperature of 2 K allows the pressure-altitude curve to be realistic, so it is replaced with a new curve from OhioBob's calculator.
* Atmosphere height increased to 19 km so that it can thin out more smoothly.
* Terrain altitude increased by about x4, to a new maxium altitude of 1000 m. This makes for taller but somewhat less steep hills.
* Adiabatic index increased to 11. This is not realistic, but it maintains the distinctive feature of Jones that the speed of sound is just less than orbital velocity.
* The increase to Jones's radius and terrain altitudes could destroy any craft saved in Jones's SOI before applying the patch.

#### Selectable spoilers
If you have already found [REDACTED], this patch lets you find it again more easily by clicking [REDACTED] in the [REDACTED].

(This is intentionally vague because it's a big spoiler.)
