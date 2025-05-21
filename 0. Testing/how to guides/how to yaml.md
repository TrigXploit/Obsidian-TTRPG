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



### 3. **Object with custom keys** ❌ (YAML valid, but not great for Dataview)

```
list:
  1st: value
  2nd: value
```
This is **valid YAML**, but:
- Not really a list — it's a map (object) with keys `"1st"` and `"2nd"`.
- Hard to loop or sort in Dataview.
- Not recommended unless you have a specific reason.



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



### 6. **Link and Metadata Objects**
```
allies:
  - name: [[John Doe]]
    role: friend
    level: 2
```
**Great for:** Combining links and data. Use `dv.table()` to show links with context.

