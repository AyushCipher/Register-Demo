# 🚀 NxtWave — Build Your First AI Project

An interactive, modern, high-performance landing page and referral engine built for **NxtWave's AI Workshop**. 

Features an interactive procedural HTML5 Canvas 3D space visualizer, real-time referral tracking dashboard, reward unlocking mechanism, Google Meet 1:1 slot booking modal, and celebratory particle confetti.

---

## ✨ Features

- 🌌 **Scroll-Driven 3D Canvas Visualizer**: Procedurally rendered particle vortex, pulsating rings, satellite nodes, and glowing core drawn at 60 FPS without external heavy 3D library overhead.
- ⚡ **Dynamic Registration & Referral Engine**:
  - Instant client-side validation and personalized dashboard generation.
  - Unique referral link generator (`nxtwave.io/workshop?ref=NW-XXXX`).
  - Native 1-click sharing to WhatsApp, LinkedIn, and Twitter/X.
  - Interactive "Simulate Friend Register" feature for immediate demonstration of the referral milestone progression.
- 🎁 **Milestone Unlock System**:
  - Live progress dots tracking towards the goal of 3 friends.
  - Unlocks a free 1:1 AI Resume Review mentorship session (valued at ₹4,999) with celebratory confetti canvas animation.
- 📅 **Google Meet Booking Modal**: Interactive calendar slot selector and immediate booking confirmation for mentorship sessions.
- 📱 **Fully Responsive & Dark-Themed**: Handcrafted responsive CSS grid and flexbox layout with ultra-sleek glassmorphism and custom interactive cursor.
- ⚡ **Zero External Dependencies Required**: Completely self-contained, light, fast, and ready to deploy anywhere.

---

## 📂 Project Structure

```text
nxtwave-project/
├── index.html          # Primary entry point (Production-ready web app)
├── nxtwave-final.html  # Standalone template backup
├── server.js           # Built-in zero-dependency local Node.js static server
├── package.json        # NPM scripts for running and tooling
├── vercel.json         # Vercel routing, clean URLs & security headers configuration
├── .gitignore          # Git ignore rules for node_modules, cache, logs, and build artifacts
└── README.md           # Documentation, run guides, and deployment instructions
```

---

## 🏃 How to Run Locally

You can run this project locally using any of the following methods:

### Option 1: Using Node.js (Recommended)
No `npm install` needed — `server.js` uses native Node.js libraries:

```bash
# Start the local server
npm start
```
*or directly with Node:*
```bash
node server.js
```
Open **[http://localhost:3000](http://localhost:3000)** in your browser.

---

### Option 2: Using Python
If you have Python installed:

```bash
# Python 3
python -m http.server 3000
```
Open **[http://localhost:3000](http://localhost:3000)** in your browser.

---

### Option 3: Direct Browser Launch
Because all logic, styling, canvas drawing, and SVGs are self-contained, you can also directly open `index.html` in any modern web browser (Google Chrome, Microsoft Edge, Firefox, Brave, Safari) by double-clicking it or running:

```powershell
Start-Process index.html
```

---

## 🐙 How to Upload to GitHub

1. **Create a new repository on GitHub**:
   - Go to [github.com/new](https://github.com/new).
   - Enter repository name: `nxtwave-ai-workshop` (or any name you prefer).
   - Choose **Public** or **Private**.
   - Do **NOT** check "Initialize this repository with a README" (we already have all files ready).
   - Click **Create repository**.

2. **Commit and push from your terminal**:
   ```bash
   # Add all files to staging
   git add .

   # Commit changes
   git commit -m "feat: initial commit for NxtWave AI workshop landing page & referral engine"

   # Rename branch to main (if not already main)
   git branch -M main

   # Link your remote GitHub repository (replace with your repo URL)
   git remote add origin https://github.com/AyushCipher/<your-repo-name>.git

   # Push code to GitHub
   git push -u origin main
   ```

---

## 🚀 How to Deploy on Vercel

### Method 1: Deploy via Vercel Web Dashboard (Recommended & Automatic)

1. Go to [vercel.com](https://vercel.com) and log in (or sign up with your GitHub account).
2. Click **"Add New..."** ➔ **"Project"**.
3. Select your GitHub repository (`nxtwave-ai-workshop`).
4. In the configuration window:
   - **Framework Preset**: Select `Other` (or leave default).
   - **Root Directory**: `./` (default).
   - **Build and Output Settings**: Leave empty (no build step needed for static HTML/JS).
5. Click **"Deploy"**.
6. Within 10 seconds, Vercel will provide your live production URL (e.g., `https://nxtwave-ai-workshop.vercel.app`) with automatic SSL, global CDN distribution, and continuous deployment on every `git push`.

---

### Method 2: Deploy via Vercel CLI

If you prefer using the terminal:

```bash
# Run Vercel CLI directly without global install
npx vercel
```

- When prompted to set up and deploy, type `y` and press Enter.
- Choose your Vercel team/account.
- Link to existing project? Type `n`.
- Project name: `nxtwave-ai-workshop`.
- In which directory is your code located? `./`.
- Auto-detected settings: accept defaults.

For production deployment:
```bash
npx vercel --prod
```

---

## 🛠️ Technology Stack

- **HTML5 & CSS3**: Modern typography (Space Grotesk & Inter via Google Fonts), Flexbox, CSS Grid, custom radial gradients, glassmorphism, keyframe animations.
- **Vanilla JavaScript**: State-driven UI, scroll event tracking, procedural HTML5 2D Canvas rendering, dynamic confetti simulation.
- **Node.js**: Zero-dependency local development server.
- **Vercel**: Edge network hosting with custom routing and security headers.

---

## 📄 License
This project is open-source and available under the [MIT License](LICENSE).
