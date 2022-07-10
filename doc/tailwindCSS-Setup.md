#3.1 TailwindCSS Setup

## install tailwindcss

```shell
npm install -D tailwindcss postcss autoprefixer
```
- tailwindcss
- postcss
- auto autoprefixer

## init tailwindcss
```shell
npx tailwindcss init -p
```

## setup tailwindcss

### /tailwind.config.js
```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: [
      "./pages/**/*.{js,jsx,ts,tsx}",
      "./components/**/*.{js,jsx,ts,tsx}"
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

### /styles/globals.css
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```