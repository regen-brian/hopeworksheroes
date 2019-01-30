# Hopeworks Heroes
Turn Based RPG

### Monster Attributes
* Atk: Attack
* Def: Defense
* HP: Health Points
* LVL: Level
* crit: Critical Attack Rate
* crdmg: Critical Attack Multiplier

###Attack Formula
* Defense - Attack = Damage
* if target's defense is greater or equal to the attackers attack the damage is either 1 or 2 damage
* upon attack we will generate a random number between 1-100 and if the number is less than or equal to the crit it will add the crdmg percentage times the damage to the total damage
