# Setting Up tailwind CSS the way I like it 

## Plain HTML

```bash
npm install -D tailwindcss
npx tailwindcss init
    
```
Paste this into your tailwind config 


```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

> I dont use a src folder


Paste this into your css file

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
 ```
To start watching the files run
```bash
npx tailwindcss -i ./{index.css} -o ./dist/{output.css} --watch
```
Replace index and output with whichever files you want to be your input and output

Link the output.css file to the html page you want to style


I know this looks alot like the tailwind css documentation but the goal of this is to eventually write an automation script for this, react and nextjs setup.

Till next time ...

