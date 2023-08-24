## All Projects by status

```dataview
LIST rows.file.link
FROM "01-Jellyfish"
WHERE type="Project"
SORT file.name ASC
GROUP BY status
```
