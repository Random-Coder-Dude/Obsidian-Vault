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
const calendarData = {
  colors: {
    green: ["#c6e48b", "#7bc96f", "#49af5d", "#2e8840", "#196127"],
  },
  showCurrentDayBorder: true,
  entries: []
};

// Count how many notes were edited on each day
const editCounts = {};

for (let page of dv.pages().where(p => p.file && p.file.mtime)) {
  const date = page.file.mtime.toFormat("yyyy-MM-dd");
  editCounts[date] = (editCounts[date] || 0) + 1;
}

// Add to calendarData
for (let date in editCounts) {
  calendarData.entries.push({
    date: date,
    intensity: editCounts[date],
    color: "green"
  });
}

renderHeatmapCalendar(this.container, calendarData);
```

```

``` dataview
table file.mtime as "Last Modified"
from ""
sort file.mtime desc
limit 10
```
