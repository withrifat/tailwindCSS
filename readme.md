🚀 Tips for Installing Tailwind CSS with Bun & Vite (Vanilla JS)
A quick guide to set up Tailwind CSS using Bun and Vite for a Vanilla JavaScript project.

⚙️ Step 1: Create Your Project
bash
Copy
Edit
bun create vite@latest .
npm i -g bun
When prompted, select "Vanilla" for the framework.

📦 Step 2: Install Dependencies
bash
Copy
Edit
bun install
bun run dev
🎨 Step 3: Install Tailwind CSS
bash
Copy
Edit
bun add tailwindcss @tailwindcss/vite
🛠️ Step 4: Configure Vite
Create a file named vite.config.ts in the root directory and add the following:

ts
Copy
Edit
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [
    tailwindcss(),
  ],
})
💅 Step 5: Set Up Tailwind in CSS
Inside your css folder:

Delete all existing styles.

Create a new file (e.g., main.css) and add:

css
Copy
Edit
@import "tailwindcss";
🧪 Final Step: Run the Project
bash
Copy
Edit
bun run dev