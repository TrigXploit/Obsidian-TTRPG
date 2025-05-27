---
Art: "![Robin Wolf pic.jpg]"
Type: Player
Level: "2"
proficiency_bonus: 2
speed: 30
HP: 15
Dex_bonus: 4
Wis_bonus: 3
Int_bonus: 2
Con_bonus: 1
Str_bonus: 0
Cha_bonus: -1
Base_AC: 14
Darkvision: 60
---

>[!column|3 flex no-t]
>> [!infobox|flex]
>> # `=this.file.name`
>> ![[Robin Wolf pic.jpg | hs-med]]
>> 
>> ###### Stats
>>  |
>> ---|---|
>> **Level** |`=this.level` |
>>  **Speed** |`=this.speed` |
>> **Proficiency** | +`=this.proficiency_bonus` |
>> **Initiative** | +`=this.Dex_bonus` |
>> **AC** | `=(this.Base_AC + this.Dex_bonus)`
>> **HP** | `=this.HP - this.DmgTkn + this.TempHP` |
>> **Hit Dice** | `=this.Level + this.HitDice`  |
>> **Passive Perception** | `=(10 + this.Wis_bonus + (this.proficiency_bonus * 2))`
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
>
> > [!infobox|flex wsmall]
>> ###### My Stuff
>> Copper | Silver | Gold | Platinum |
>> ---|---|---|---|
>> 1|2|3|4|
>> 
>> ![[Tables#Equipment]]
>> ![[Tables#inventory]]
>
>
>> [!infobox|flex wsmall]
>> # Combat
>> ###### Spells
>> ![[Tables#spells]]
>> ###### Attacks
>
>



