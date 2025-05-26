---
Type: Player
Art: "![[Robin Wolf pic.jpg]]"
Level: 0
AC: 0
Prof: 
HP: 0
HitDice: d0
Speed: 0
STR: 0
DEX: 0
CONST: 0
INT: 0
WIS: 0
CHA: 0
Race: RaceName
Alignment: NONE
Gender: GenderName
Age: "0"
Location: NONE
Class: ClassName
Subclass: SubClassName
AssociatedGroup: NONE
Likes: NONE
Dislikes: NONE
Pronouns: NONE
PersonalityTrait:
  - NONE
SocialTrait:
  - NONE
MentalTrait:
  - NONE
Proficiencies:
  - NONE
Resistances:
  - NONE
Languages:
  - NONE
DmgTkn: 0
TempHP: 0
Copper: 0
Silver: 0
Electrum: 0
Gold: 0
Platinum: 0
---
>[!column|flex 2]
>> [!infobox| wtall]
>> # `=this.file.name`
>> ![[Robin Wolf pic.jpg | hs-med]]
>> 
>> ###### Stats
>>  |
>> ---|---|
>> **Level** |`=this.level` |
>>  **Speed** |`=this.Speed` |
>> **Proficiency** | +`=this.Prof` |
>> **Initiative** | +`=(this.DEX - 10)/2` |
>> **AC** | `=this.AC`
>> **HP** | `=this.HP - this.DmgTkn + this.TempHP` |
>> **Hit Dice** | `=this.Level + this.HitDice`  |
>> **Passive Perception** |
>>  
>> ###### Bio
>>   |
>> ---|---|
>> **Race** | `=this.race` |
>> **Sex** | `=this.gender` |
>> **Age** | `=this.age` |
>> **Sexuality** | `=this.sexuality` |
>> **Alignment** | `=this.alignment` |
>> ###### Info
>>   |
>> ---|---|
>> **Class(s)** | `=this.Class` |
>> **Sub-Class(s)** | `=this.Subclass`
>> **Group(s)** | `=this.AssociatedGroup` |
>> **Religion(s)** | `=this.AssociatedReligion` |
>> **Current Location** | `=this.Location` |
>
>> [!infobox | wtall] Death Saves
>> ### Death Saves
| Success | <input type="checkbox" unchecked>  | <input type="checkbox" unchecked> | <input type="checkbox" unchecked> | 
| ------- | --- | --------------------------------- | --------------------------------- |
>>
| Fails | <input type="checkbox" unchecked>  | <input type="checkbox" unchecked> | <input type="checkbox" unchecked> | 
| ----- | --- | --------------------------------- | --------------------------------- |
>>
>> ### Skills
| Skill | Score       | Mod                     | Prof                              | ST                                  |
| ----- | ----------- | ----------------------- | --------------------------------- | ----------------------------------- |
| <font color="#ff0000">**STR**</font>   | `=this.STR` | +`=(this.STR - 10)/2`   | <input type="checkbox" unchecked> | +`=(this.STR - 10)/2`               |
| <font color="#ffff00">**DEX**</font>   | `=this.DEX`  | +`=(this.DEX - 10)/2`   | <input type="checkbox" unchecked> | +`=(this.DEX - 10)/2`               |
| <font color="#00b050">**CON**</font>   | `=this.CONST` | +`=(this.CONST - 10)/2` | <input type="checkbox" unchecked>   | +`=((this.CONST - 10)/2)` |
| <font color="#7030a0">**INT**</font>   | `=this.INT`          | +`=(this.INT - 10)/2`   | <input type="checkbox" unchecked>   | +`=((this.INT - 10)/2)`   |
| <font color="#245bdb">**WIS**</font>   | `=this.WIS`          | +`=(this.WIS - 10)/2`   | <input type="checkbox" unchecked> | +`=(this.WIS - 10)/2`               |
| <font color="#de7802">**CHA**</font>   | `=this.CHA`          | +`=(this.CHA - 10)/2`   | <input type="checkbox" unchecked> | +`=(this.CHA - 10)/2`               |
>> ![[Tables#currency]]
>> ![[Tables#inventory]]
>> ![[Tables#Equipment]]


a