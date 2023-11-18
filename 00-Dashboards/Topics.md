## Notes by topic

Excludes fleeting notes.

### Active, Holding, Planned, Maybe

```dataview
TABLE sort(rows.file.link) AS "Note"
FROM "01-Jellyfish"
WHERE status!="Archive" AND type!="Fleeting"
FLATTEN topic
GROUP BY topic
```

### Archive

```dataview
TABLE sort(rows.file.link) AS "Note"
FROM "01-Jellyfish"
WHERE status="Archive" AND type!="Fleeting"
FLATTEN topic
GROUP BY topic
```
