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

``` dataviewjs
const year = 2025;  // change as needed
const startOfYear = moment(`${year}-01-01`).startOf('year');
const endOfYear = moment(`${year}-12-31`).endOf('year');

const trackerData = {
    year: year,
    entries: [],
    separateMonths: true,
    heatmapTitle: "Daily Notes Edited",
    heatmapSubtitle: `Notes edited per day in ${year}`,
    colorScheme: {
        paletteName: "Serge 1",
    },
    defaultEntryIntensity: 0,
    intensityScaleStart: 0,
    intensityScaleEnd: 10  // max expected notes per day — adjust as needed
};

// Map to count notes edited per date string
const editCounts = new Map();

// Gather all pages modified within the year
for (let page of dv.pages()) {
    if (!page.file || !page.file.mtime) continue;
    const mtime = moment(page.file.mtime);
    if (mtime.isBefore(startOfYear) || mtime.isAfter(endOfYear)) continue;

    const dateStr = mtime.format("YYYY-MM-DD");
    editCounts.set(dateStr, (editCounts.get(dateStr) || 0) + 1);
}

// Convert map to trackerData.entries array
for (const [date, count] of editCounts) {
    trackerData.entries.push({
        date: date,
        intensity: count,
        content: null  // you can add links or summaries if you want, else null
    });
}

// Render heatmap
renderHeatmapTracker(this.container, trackerData);
```


``` dataview
table file.mtime as "Last Modified"
from ""
sort file.mtime desc
limit 10
```

