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
current_Blood_pool: 9
max_blood_pool: 13
merits:
  - name: Big
    points: 3
  - name: Strong
    points: 3
flaws:
  - name: Blind
    points: 3
  - name: Mute
    points: 2
---
>[!infobox|no-table-header ]+  
># Loui
>![[Loui image.jpg|]]
>
>>[!Current-Stats]+
>>**Blood Pool:** `=this.current_blood_pool` / `=this.max_blood_pool`
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


```button
name: +1 Blood
type: meta
action: update
args:
  field: current_blood_pool
  value: "{{value + 1}}"

## Abilities
