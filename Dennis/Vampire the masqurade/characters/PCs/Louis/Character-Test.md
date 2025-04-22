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
  talents: Alertness Athletics Awareness
  skills: Animal-ken Crafts Drive
  knowledges: Academics Computer Finance
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
humanity: 5
willpower: 5
max_blood_pool: 13
current_blood_pool: 12
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

>[!infobox|no-table-header ws-med]+  
># Loui
>![[Loui image.jpg|]]
>
>>[!Current-Stats]+
>>**Blood Pool:** 
>>```meta-bind
>>INPUT[number:current_blood_pool]
>>```
>>a
>>  **Blood Pool:** `VIEW[{current_blood_pool}]` / `VIEW[{max_blood_pool}]` `BUTTON[blood-increment, blood-reset, blood-decrement]`
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
>>**Disciplines** | Animalism<br>Fortitude<br>Protean |
>


## Attributes

> [!col| ]
>> [!col-md]
>> ### Physical
>>type|value|
>> ---|---| 
>>test1|test 1|
>
>> [!col-md]
>> ### Social
>>type|value|
>> ---|---| 
>> test2|test 2|
>
>> [!col-md]
>> ### Mental
>> type|value|
>> ---|---| 
>> test3|test 3| 


## Abilities

> [!col|no-table-header ]
>> [!col-md]
>>```dataviewjs
>>const attrs = dv.current().attributes.physical;
>>dv.table(["Physical", "Value"],
> > Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>>)
>>```
>
>> [!col-md]
>>```dataviewjs
>>const attrs = dv.current().attributes.social;
>>dv.table(["Social", "Value"],
>>  Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>>)
>>```
> 
> 
>> [!col-md]
>>```dataviewjs
>>const attrs = dv.current().attributes.mental;
>>dv.table(["Mental", "Value"],
>>  Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>>)
>>```






testing

> [!column]
>> [!info] Column 1
>> - Use another callout for columns
>
>> [!note] Column 2
>> Need that singular blockquote `>` as separation between columns


> [!col|]
>
>> [!col-md] 
>> ### Physical
>> 
>> ```dataviewjs
>> const attrs = dv.current().attributes.physical;
>> dv.table(["Type", "Value"],
>>   Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>> )
>> ```
>
>> [!col-md]
>> 
>> ### Social
>> ```dataviewjs
>> const attrs = dv.current().attributes.social;
>> dv.table(["Type", "Value"],
>>   Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>> )
>> ```
>
>> [!col-md]
>> 
>> ### Mental
>> ```dataviewjs
>> const attrs = dv.current().attributes.mental;
>> dv.table(["Type", "Value"],
>>   Object.entries(attrs).map(([key, val]) => [key, "●".repeat(val)])
>> )
>> ```
