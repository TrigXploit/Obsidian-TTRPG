### 1. **Nested Object (map of maps)** ✅

```
listOfObjects:
  object1:
    konstant1: value
    konstant2: value
  object2:
    konstant1: value
    konstant2: value

```
**Good for:** Grouping known keys with sub-values.  
**Access in `dataviewjs`:** `dv.current().listOfObjects.object1.konstant1`



### 2. **List of Objects** ✅
```
listOfObjects:
  - objectName: value1
    konstant1: value
    konstant2: value
  - objectName: value2
    konstant1: value
    konstant2: value
```
**Good for:** Lists where each item has multiple named properties.  
**Access in `dataviewjs`:** Loop with `.map()`, e.g. `dv.current().listOfObjects.map(o => o.objectName)`

> ⚠️ `objectName` here is just another property — not a true key name. If you want it to **act like a name**, call it `name:` instead of `objectName:` for clarity.



### **Flat map** ✅ (good for numeric or uniform data)

```
map:
  1st_Key: value
  2nd_Key: value
```
*important note:*
- keys have to be content (something you care about).



### 4. **List of strings** ✅

```
list:
  - "This is the 1st thing in the list"
  - "This is the 2nd thing in the list"
```
**Good for:** Simple lists of items.  
**Access in `dataviewjs`:** `dv.current().list.map(item => ...)`



### 5. **Flat Key-Value Pairs (Simple Fields)**
```
clan: Gangrel
generation: 10
```