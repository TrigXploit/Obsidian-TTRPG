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
current_blood_pool: 8
max_blood_pool: 13
count: 0
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
>[!infobox|no-table-header ]+  
># Loui
>![[Loui image.jpg|]]
>
>>[!Current-Stats]+
>>**Blood Pool:** 
>>```meta-bind
>>INPUT[number:current_blood_pool]
>>```
>>
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


## Attributes

## Abilities


```meta-bind-button
label: "+1"
hidden: true
id: "count-increment"
style: default
actions:
  - type: updateMetadata
    bindTarget: count
    evaluate: true
    value: "x + 1"
```

```meta-bind-button
label: "-1"
hidden: true
id: "count-decrement"
style: default
actions:
  - type: updateMetadata
    bindTarget: count
    evaluate: true
    value: "x - 1"
```

```meta-bind-button
label: "Reset"
hidden: true
id: "count-reset"
style: default
actions:
  - type: updateMetadata
    bindTarget: count
    evaluate: false
    value: 0
```

`BUTTON[count-decrement, count-reset, count-increment]` `VIEW[{count}]`

