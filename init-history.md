# INIT HISTORY

## Create Vite & React TS Template

```
npm create vite@latest . -- --template react-ts
```

<!-- code markup -->

## Install Sass

```
npm install sass
```

## Tailwinds

```
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

## tailwind.config.js

```
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

## src/index.css

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

VS Code PostCSS Language Support

- Extenstions (cmd + shift + x)
- Search "PostCSS Language Support"

## Set Prettier

```
npm install -D prettier eslint-config-prettier eslint-plugin-prettier
```

1.  Add `.prettierrc`

```
{
  "semi": false,
  "singleQuote": false,
  "tabWidth": 2,
  "trailingComma": "es5",
  "printWidth": 100,
  "bracketSpacing": true,
  "arrowParens": "always",
  "endOfLine": "auto"
}
```

2. Install Extension: Prettier - Code formatter
3. settings.json

```
{
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true
}
```

4. `.prettierignore`

```
dist
node_modules
```
