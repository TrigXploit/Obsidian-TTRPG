---
Art: "![Robin Wolf pic.jpg]"
Type: Player
Level: 3
proficiency_bonus: 2
speed: 30
HP: 21
Dex_bonus: 4
Wis_bonus: 3
Int_bonus: 2
Con_bonus: 1
Str_bonus: 0
Cha_bonus: -1
Base_AC: 13
Darkvision: 60
Hit_Dice: 8
Classes:
  - "lv 1 [[1.Rouge|Rouge]]"
  - "lv 2 [[1.Cleric|Cleric]]"
Sub-Class:
  - "[[Assassin]]"
  - "[[Hunt Domain (Heliana_s Guide to Monster Hunting)|Hunt Domain]]"
Feats:
  - "[[Feats#Expert Harvester|Expert Harvester]]"
---

>[!column|3 flex no-t]
>> [!infobox|flex]
>> # `=this.file.name`
>> ![[Robin Wolf pic.jpg | hs-med]]
>> 
>> ###### Stats
>>  |
>> ---|---|
>> **Level** |`=this.Level` |
>> **Speed** |`=this.speed` |
>> **Proficiency** | +`=this.proficiency_bonus` |
>> **Initiative** | +`=this.Dex_bonus` |
>> **AC** | `=(this.Base_AC + this.Dex_bonus)`
>> **HP** | `=this.HP` |
>> **Hit Dice** | `=this.Level`d`=this.Hit_Dice`  |
>> **Passive Perception** | `=(10 + this.Wis_bonus + (this.proficiency_bonus*2))`
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
>> **Class(s)** | `=this.Classes` |
>> **Sub-Class(s)** | `=this.Sub-Class`
>> **Feat(s)**|`=this.Feats`
>> **Harvesting** | 
>> **Assessment** | 1D20 + `=this.Int_bonus` + `=2*this.proficiency_bonus`
>> **Carving** | 1D20 + `=this.Dex_bonus` + `=2*this.proficiency_bonus`
>> **Group(s)** | `=this.AssociatedGroup` |
>> **Current Location** | `=this.Location` |
>> ![[Tables#Group Currency]]
>
>
>> [!infobox|flex wsmall]
>> ###### My Stuff
>> ![[Tables#Fenra currency]]
>> 
>> ![[Tables#Fenra Equipment]]
>> ![[Tables#Fenra inventory]]
>
>
>> [!infobox|flex wsmall]
>> ###### Spells
>> ![[Tables#spells]]
>> ###### Attacks
>> ![[Tables#Actions]]
>