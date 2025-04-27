# 🎨 Tailwind CSS Setup with Bun + Vite + Vanilla JS

This guide walks you through setting up **Tailwind CSS** in a **Vanilla JavaScript** project using **Bun** and **Vite**.

---

## 🧱 Step 1: Create a New Project

```bash
bun create vite@latest .
npm i -g bun  # Install Bun globally if not already installed
✅ When prompted, choose "Vanilla" for the framework.

📦 Step 2: Install Dependencies
bash
Copy code
bun install
bun run dev
🎨 Step 3: Install Tailwind CSS
bash
Copy code
bun add tailwindcss @tailwindcss/vite
⚙️ Step 4: Configure Vite for Tailwind
Create a file named vite.config.ts in the root directory and add:

ts
Copy code
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [tailwindcss()],
})
🛠️ Step 5: Initialize Tailwind Config
Run the following to generate a tailwind.config.js file:

bash
Copy code
bunx tailwindcss init
Update it to:

js
Copy code
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ['./index.html', './src/**/*.{js,ts}'],
  theme: {
    extend: {},
  },
  plugins: [],
}
💅 Step 6: Set Up CSS
In your main CSS file (e.g., style.css), clear everything and add:

css
Copy code
@import "tailwindcss";
🚀 Step 7: Start the Dev Server
bash
Copy code
bun run dev
