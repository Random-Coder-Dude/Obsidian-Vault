<%*
const folderPath = tp.file.folder(true); // e.g. "1000 - Science/1100 - Chemistry/..."
const folderParts = folderPath.split("/"); // Split correctly using "/"

const targetFolderRaw = folderParts.length >= 2 ? folderParts[1] : "root"; // second-highest (index 1)
const cleanedFolder = targetFolderRaw.replace(/^\d+\s*-\s*/, ""); // Remove leading digits and dash

tR += "---\n";
tR += "date: " + tp.date.now("YYYY-MM-DD") + "T" + tp.date.now("HH:mm") + "\n";
tR += "tags:\n";
tR += `  - ${cleanedFolder}\n`;
tR += "cssclasses:\n";
tR += "  - default\n";
tR += "---\n";
%>
