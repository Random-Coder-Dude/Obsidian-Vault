<%*
const fileFolder = tp.file.path(true);
const folderParts = fileFolder.split("/");

// Get the second-highest folder, if available
const secondHighest = folderParts.length > 1 ? folderParts[1] : (folderParts[0] || "root");

// Remove leading numbers and dashes (e.g. '01-Chapter' -> 'Chapter')
const cleanedFolder = secondHighest.replace(/^\d+-?/, "");

tR += "---\n";
tR += "date: " + tp.date.now("YYYY-MM-DD") + "T" + tp.date.now("HH:mm") + "\n";
tR += "tags:\n";
tR += `  - ${cleanedFolder}\n`;
tR += "cssclasses:\n";
tR += "  - default\n";
tR += "---\n";
%>
