---
name: Loui
player: Marcus
clan: Gangril
sect: Camarilla
generation: 10
sire: Lebron James
concept: Underground Boxer
nature: unknown
demeanor: unknown
humanity: 5
willpower: 5
max_blood_pool: 13
current_blood_pool: 12



attributes:
  physical:
    strength: 3
    dexterity: 3
    stamina: 3
  social:
    Charisma: 3
    manipulation: 3
    appearance: 3
  mental:
    perception: 3
    intelligence: 3
    wits: 3


abilities:
  talents: 
    Alertness: 1 
    Athletics: 2
    Awareness: 3
  skills: 
    Animal-ken: 1
    Crafts: 2
    Drive: 3
  knowledges: 
    Academics: 1
    Computer: 2
    Finance: 3


disciplines:
  - animalism
  - fortitude
  - protean


virtues:
  conscience: 4
  self_control: 3
  courage: 5


backgrounds:
  - resources: 2
  - allies: 1


merits:
  - name: big
    points: 3
  - name: strong
    points: 3


flaws:
  - name: blind
    points: 3
  - name: mute
    points: 2
---
```meta-bind-button
label: "+1"
hidden: true
id: "blood-increment"
style: default
actions:
  - type: updateMetadata
    bindTarget: current_blood_pool
    evaluate: true
    value: "x + 1"
```

```meta-bind-button
label: "-1"
hidden: true
id: "blood-decrement"
style: default
actions:
  - type: updateMetadata
    bindTarget: current_blood_pool
    evaluate: true
    value: "x - 1"
```

```meta-bind-button
label: "Reset"
hidden: true
id: "blood-reset"
style: default
actions:
  - type: updateMetadata
    bindTarget: current_blood_pool
    evaluate: true
    value: "getMetadata('max_blood_pool')"
```
>[!infobox|no-table-header  wsmall]+  
># Loui
>![[Loui image.jpg|]]
>
>>[!Current-Stats]+
>>**Blood Pool:** 
>>```meta-bind
>>INPUT[number:current_blood_pool]
>>```
>>a
>>  **Blood Pool**`VIEW[{current_blood_pool}]` / `VIEW[{max_blood_pool}]` `BUTTON[blood-increment, blood-reset, blood-decrement]`
>>a
>>**Willpower**  
>>```meta-bind
>>INPUT[number:willpower]
>>```
>
>>[!Bio]+
>>Type |  value |
>> ---|---|
>>**player**|Marcus|
>>**Clan**|Gangril| 
>>**Generation**| 10|  
>>**Sect**| Camarilla|  
>>**Sire**| sheriff <br>Lebron James |  
>>**Concept**| Underground Boxer  |
>>**Nature**| unknown | 
>>**Demeanor**| unknown  |









## Attributes

> [!column| 3 no-t  ]
>> [!blank|no-table-header wm-tl] Column 1
>> ### Physical
>> ```dataviewjs
>>const attrs = dv.current().attributes.physical;
>>dv.table(["Physical", "Value"],
> > Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>>)
>>```
>
>> [!blank|no-table-header wm-tl] Column 2
>> ### Social
>>```dataviewjs
>>const attrs = dv.current().attributes.social;
>>dv.table(["Social", "Value"],
>>  Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>>)
>>```
>
>> [!blank|no-table-header wm-tl] Column 3
>> ### Social
>>```dataviewjs
>>const attrs = dv.current().attributes.mental;
>>dv.table(["Mental", "Value"],
>>  Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>>)
>>```
>





## Abilities

> [!col|no-table-header ]
>> [!col-md| ]
>> ```dataviewjs
>> const attrs = dv.current().abilities.talents;
>> dv.table(["Physical", "Value"],
>> Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>> )
>
>> [!col-md]
>>```dataviewjs
>>const attrs = dv.current().abilities.skills;
>>dv.table(["Social", "Value"],
>>  Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>>)
>>```
> 
>> [!col-md]
>>```dataviewjs
>>const attrs = dv.current().attributes.mental;
>>dv.table(["Mental", "Value"],
>>  Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>>)
>>```


## Advantages
> [!col|no-table-header ]
>> [!col-md| ]
>>const attrs = dv.current().advantages