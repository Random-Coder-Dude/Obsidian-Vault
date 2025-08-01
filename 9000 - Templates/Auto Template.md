<%*
const fileFolder = tp.file.path(true);
const topLevelFolder = fileFolder.includes("/") ? fileFolder.split("/")[0] : (fileFolder || "root");

tR += "---\n";
tR += "date: " + tp.date.now("YYYY-MM-DD") + "T" + tp.date.now("HH:mm") + "\n";
tR += "tags:\n";
tR += `  - ${topLevelFolder}\n`;
tR += "cssclasses:\n";
tR += "  - default\n";
tR += "---\n";
%>