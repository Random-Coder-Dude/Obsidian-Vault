<%*
tR += "---\n";
tR += "date: " + tp.date.now("YYYY-MM-DD") + "T" + tp.date.now("HH:mm") + "\n";
tR += "tags:\n  - Daily\n";
tR += "cssclasses:\n  - daily\n  - " + tp.date.now("dddd").toLowerCase() + "\n";
tR += "---\n\n";
%>

<% tp.web.daily_quote() %>
# DAILY NOTE  
## <% tp.date.now("dddd, MMMM Do, YYYY") %>  
***  
### Tasks Completed
