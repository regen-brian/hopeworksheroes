# Hopeworks Heroes
Turn Based RPG

### Monster Attributes
#### Heroes
* name: Hero Name, Cannot change, Can have same as others
* class: Each class has different passives & attacks, Cannot change
* bio: Can choose a prefilled backstory or create their own
* battle cry: Can type their own
* hair color: Changeable
* clothes color: Changeable
* skin color: Changeable
* gender: Cannot change
* lvl: Current level of hero
* xp: Current total experience points of hero
* hp: Health Points
* atk: Attack
* def: Defense
* crit: Critical Attack Rate
* crdmg: Critical Attack Multiplier

#### Enemies
* name: Enemy Name
* type: Description of enemy
* xpType: A flag to determine the multiplier for experience points given if defeated. Common = 0, Rare = +30%
* lvl: Current level of enemy
* hp: Health Points
* atk: Attack
* def: Defense
* crit: Critical Attack Rate
* crdmg: Critical Attack Multiplier


### Attack Formula
* Defense - Attack = Damage
* if target's defense is greater or equal to the attackers attack the damage is either 1 or 2 damage
* upon attack we will generate a random number between 1-100 and if the number is less than or equal to the crit it will add the crdmg percentage times the damage to the total damage

### Leveling Mechanics
* We will use an object to define amounts of xp for each level
* Level 1 will give 100xp and any level after that will increase by 10%
* There are 2 types of enemies, common and rare. Rare enemies will give a 50% boost to xp
