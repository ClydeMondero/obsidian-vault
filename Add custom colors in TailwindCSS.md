[[TailwindCSS]]

# Add custom colors in TailwindCSS
#resource 

tailwind.config.js
```js
 module.exports = {
  theme: {
    extend: {
      colors: {
        'black-rgba': 'rgba(0, 0, 0, 0.54)',
      },
    },
  },
  variants: {},
  plugins: [],
}
```

```html
<span class="text-black-rgba text-4xl">Hi there!</span>
```

[Reference](https://stackoverflow.com/a/65307983)