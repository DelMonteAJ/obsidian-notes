```dataviewjs
for (let group of dv.pages("#projects").groupBy(p => p.status)) {
	dv.header(3, group.key);
	dv.table(["Name", "Description", "Link"],
		group.rows
			.sort(k => k.name, 'desc')
			.map(k => [k.file.link, k["description"], k.link]))
}

```



### All Projects
```dataview
TABLE Description, Link, Status
FROM #projects
SORT file.name ASC
```