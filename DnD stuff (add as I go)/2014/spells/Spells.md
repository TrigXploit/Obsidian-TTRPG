noterpad commands:
##### to clean tables
```
#remove hyperlink
\[(.*?)\]\(https://dnd5e\.wikidot\.com/spell:[^)]*\)
#replace with
\1
```

##### To clean Duration
```
Instantaneous 

#replace with
Instant
```

```
Concentration,\s*(up to [^|]+)\|\s*([VSM,\s]+)


#replace with

##use mathematica
\1| C, \2

```

##### to list each Spell
```
#replace 1st space with ###
^ (\S.*)

#replace with
### \1
```

## Index

[[1. cantrips]]
[[2. 1st Lv spells]]
[[3. 2nd Lv spells]]
[[4. 3rd Lv spells]]
[[5. 4th Lv spells]]
