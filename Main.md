---
banner: https://i.redd.it/a3ftzqi7ide71.png
cssclasses:
  - homepage
---
# 🎓 Academic Research Hub

>[!quote] Quote
	> **Productivity** is never an **accident**. It is always the result of a **commitment** to excellence, intelligent planning, and focused **effort**.
> &mdash; <cite>Paul J. Meyer</cite>✍️
---
# Hop In!

```dataviewjs
// Settings
const useFrontmatterDate = false; // We're using file.mtime now
const startDate = moment().startOf("year");
const today = moment();
const days = today.diff(startDate, "days") + 1;

// Build date-to-count map
let contributions = new Map();
dv.pages()
  .where(p => p.file.mtime) // Only include files with modified times
  .forEach(page => {
    const date = moment(page.file.mtime);
    const dateStr = date.format("YYYY-MM-DD");
    contributions.set(dateStr, (contributions.get(dateStr) || 0) + 1);
  });

// Build heatmap grid
let html = '<div class="contrib-graph">';
for (let i = 0; i < days; i++) {
  const date = moment(startDate).add(i, "days");
  const dateStr = date.format("YYYY-MM-DD");
  const count = contributions.get(dateStr) || 0;
  const level = count >= 5 ? 4 : count >= 3 ? 3 : count >= 2 ? 2 : count >= 1 ? 1 : 0;
  html += `<div class="contrib-day level-${level}" title="${dateStr}: ${count}"></div>`;
}
html += "</div>";
dv.container.innerHTML = html;
```

``` dataview
table file.mtime as "Last Modified"
from ""
sort file.mtime desc
limit 10
```
