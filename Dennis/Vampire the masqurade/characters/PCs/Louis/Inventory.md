---
inventory:
  - name: Potion
    quantity: 3
    note: Heals 1d4 HP
  - name: Sword
    quantity: 1
    note: Steel blade
---

## Inventory

```meta-bind-button
id: add-inventory-item
label: "Add Item"
style: primary
actions:
  - type: updateMetadata
    bindTarget: inventory
    evaluate: true
    value: "x == null ? [{name: ´New Item´, quantity: 1, note: ``}] : [...x, { name: 'New Item', quantity: 1, note: '' }]"
```

```dataviewjs
const inventory = dv.current().inventory || [];

dv.table(["Name","Quantity","Note","Edit"],
	inventory.map((item,index)=> {
		return [
			item.name,
			item.quantity,
			item.note,
			`INPUT[text:inventory[${index}].name] INPUT[number:inventory[${index}].quantity] INPUT[text:inventory[${index}].note]`
		];
	})
);	
```

`BUTTON[add-inventory-item]`
