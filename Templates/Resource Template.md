[[_005 Inbox MOC]]

<%* 
let title; 
if(tp.file.title.startsWith("Untitled")) { 
	title = await tp.system.prompt("Note name", "", true);
	 if (!(title == "")) { 
		 await tp.file.rename(title);
	} else {}; 
} else {
	title = tp.file.title;
};
_%>

# <% title %>
#resource 

[Reference]() [[Resource Template|Reference]]