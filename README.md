# Install Tailwind CSS
---

```markdown
# ⚡ Tailwind CSS Starter (CLI Setup)

A simple and clean starter template using **Tailwind CSS** with the official CLI. Ideal for small projects, prototypes, or learning Tailwind fast.

---

```

````

---

## ⚙️ Setup Instructions

### 1. Initialize your project

```bash
npm init -y
````

### 2. Install Tailwind CSS

```bash
npm install -D tailwindcss
```

### 3. Generate config file

```bash
npx tailwindcss init
```

---

## 🧾 Create CSS Input File

Create a file at: `src/input.css`

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---

## 📜 Update `package.json` Scripts

```json
"scripts": {
  "build": "npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch"
}
```

---

## 🚀 Build Your CSS

Start watching and building Tailwind CSS automatically:

```bash
npm run build
```

Or directly (without a script):

```bash
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

---

## 🌐 Sample HTML

Create a file: `index.html`

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Tailwind CSS App</title>
  <link href="./dist/output.css" rel="stylesheet">
</head>
<body class="bg-gray-100 flex items-center justify-center h-screen">
  <h1 class="text-4xl font-bold text-blue-600">Hello Tailwind!</h1>
</body>
</html>
```

---

## 🧪 Test It

Open `index.html` in your browser. If you see styled text, Tailwind is working! 🎉

---

## 📌 Notes

* Make sure `dist/output.css` is included via `<link>` in `index.html`.
* Tailwind CLI will watch and rebuild CSS on every save when using `--watch`.

---

## ✨ That's It!

You're ready to start building beautiful UIs using Tailwind CSS. Happy coding! 💻

> Made with ❤️ by \[Avi-codesmith]
