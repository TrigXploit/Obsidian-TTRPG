---
inventory:
  - name: Potion
    quantity: 3
    note: Heals 1d4 HP
  - name: Sword
    quantity: 1
    note: Steel blade

# Temporary fields for new item input
new_item_name: 
new_item_quantity: 
new_item_note: 
---

## ➕ Add New Item

| Field   | Value |
|--------|-------|
| Name   | `= this.new_item_name` |
| Qty    | `= this.new_item_quantity` |
| Note   | `= this.new_item_note` |

```meta-bind
BUTTON[submit-new-item]
```

```meta-bind-button
id: submit-new-item
label: "Add Item"
style: default
actions:
  - type: updateMetadata
    bindTarget: inventory
    evaluate: true
    value: >
      (() => {
        const newItem = {
          name: getMetadata("new_item_name"),
          quantity: parseInt(getMetadata("new_item_quantity") || "0"),
          note: getMetadata("new_item_note")
        };
        return x ? [...x, newItem] : [newItem];
      })()
  - type: resetMetadata
    keys: [new_item_name, new_item_quantity, new_item_note]
```
