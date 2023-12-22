[[Obsidian]]

# Prompt note name in note creation in Obsidian
#resource 

```
<%* 
let title; if(tp.file.title.startsWith("Untitled")) { title = await tp.system.prompt("Note name", "", true); if (!(title == "")) { await tp.file.rename(title); } else {}; } else {}; 
_%>
```

[Reference](https://www.reddit.com/r/ObsidianMD/comments/125vc7h/note_name_prompt/) 