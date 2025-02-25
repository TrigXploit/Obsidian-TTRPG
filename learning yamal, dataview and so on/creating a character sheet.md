---
level: "2"
dot-points: "5"
attributes:
  physical:
    strength: 2
    dexterity: 3
    stamina: 4
  social:
    charisma: 2
    manipulation: 3
    composure: 4
  mental: 
   intelligence: 2
   wits: 3
   composure: 4
skills:
  athletics: 2
  animal Ken: 2
  academics: 3
  brawl: 4
  etiquette: 3
  awareness: 5
  craft: 3
  insight: 2
  finance: 5
  drive: 0
  intimidation: 4
  investigation: 1
  firearms: 2
  leadership: 1
  medicine: 5
  larceny: 2
  performance: 1
  occult: 4
  melee: 2
  persuasion: 5
  politics: 1
  stealth: 5
  streetwise: 2
  science: 4
  survival: 3
  subterfuge: 2
  technology: 1
---

  

```dataviewjs
// 1. Define a function to generate dots dynamically

function dots(value){
	return "⬤".repeat(value) + "○".repeat(5-value);
}


// 2. Get the "attributes" section from YAML in the current note

const attribute = dv.current().attributes
const skills = dv.current().skills
  

// Title: Attributes

dv.paragraph("## Attributes");

// 3. Create a table with "Physical", "Social", and "Mental" attributes

dv.table(["physical", "social", "mental"], [

	["Strength " + dots(attribute.physical.strength),
	"charisma " + dots(attribute.social.charisma),
	"Intelligence" + dots(attribute.mental.intelligence)],
	
	["dexterity " + dots(attribute.physical.dexterity),
	"manipulation " + dots(attribute.social.manipulation),
	"wits " + dots(attribute.mental.wits)],
	
	["Stamina " + dots(attribute.physical.Stamina),
	"composure " + dots(attribute.social.composure),
	"resolve " + dots(attribute.mental.resolve)]
]);

  
dv.paragraph("---");
  

dv.paragraph("## Skills");


dv.table(["skill 1", "skill 2", "Skill 3"], [
	["Athletics " + dots(skills.athletics),
	"animal Ken " + dots(skills.animal_Ken),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology)],

	["Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology)],

	["Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology),
	"Athletics " + dots(skills.Technology)]
]);
  
```

