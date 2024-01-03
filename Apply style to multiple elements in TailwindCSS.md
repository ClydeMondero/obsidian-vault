[[TailwindCSS]]

# Apply style to multiple elements in TailwindCSS
#resource 

CSS
```css
@tailwind base;
@tailwind components;
@tailwind utilities;

@layer components {
.tdata{
@apply px-2 text-lg;
}
}
```

HTML 
```html
<table id="t1">
<tr>
<td class="tdata"></td>
<td class="tdata"></td>
<td class="tdata"></td>
</tr>
</table>
```

[Reference](https://stackoverflow.com/a/71975371)