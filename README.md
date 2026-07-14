# 🚀 Irtiza Zain — Personal Portfolio

A premium, fully responsive personal portfolio website built with **React + Vite + Tailwind CSS + Framer Motion**.

![Portfolio Preview](./preview.png)

## ✨ Features

- **Dark / Light Mode** — Persisted via localStorage
- **Typing Animation** — Cycling role titles in the hero
- **Smooth Animations** — Framer Motion throughout
- **Scroll Progress Bar** — Gradient indicator at the top
- **Loading Screen** — Animated intro on first visit
- **Glassmorphism** — Frosted-glass cards and navbar
- **Fully Responsive** — Mobile-first design, tested at 375px → 1440px
- **Active Nav Links** — IntersectionObserver highlights current section
- **Mobile Drawer Menu** — Slide-in hamburger menu
- **SEO Optimised** — Full meta tags, OG tags, semantic HTML
- **Accessible** — ARIA labels, focus states, semantic elements

## 🛠️ Tech Stack

| Technology     | Purpose                      |
|----------------|------------------------------|
| React 18       | UI framework                 |
| Vite 5         | Build tool & dev server      |
| Tailwind CSS 3 | Utility-first styling        |
| Framer Motion  | Animations & transitions     |
| React Icons    | Icon library                 |
| React Scroll   | Smooth scrolling             |

## 📁 Project Structure

```
portfolio/
├── public/
│   ├── favicon.svg          ← SVG favicon
│   └── resume.pdf           ← Your resume (replace this!)
├── src/
│   ├── assets/
│   ├── components/
│   │   ├── layout/
│   │   │   ├── Navbar.jsx
│   │   │   ├── Footer.jsx
│   │   │   └── ScrollProgress.jsx
│   │   ├── sections/
│   │   │   ├── Home.jsx
│   │   │   ├── About.jsx
│   │   │   ├── Skills.jsx
│   │   │   ├── Experience.jsx
│   │   │   ├── Projects.jsx
│   │   │   ├── Education.jsx
│   │   │   ├── Certificates.jsx
│   │   │   └── Contact.jsx
│   │   └── ui/
│   │       ├── Badge.jsx
│   │       ├── LoadingScreen.jsx
│   │       └── SectionTitle.jsx
│   ├── context/
│   │   └── ThemeContext.jsx
│   ├── data/
│   │   └── portfolioData.js  ← ✅ Edit your content here!
│   ├── hooks/
│   │   └── useTypingEffect.js
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── package.json
├── vite.config.js
├── tailwind.config.js
└── postcss.config.js
```

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) **v18 or higher** — download from https://nodejs.org/

### 1. Install Node.js
Download and install Node.js from https://nodejs.org/ (LTS version recommended).

After installing, verify in a terminal:
```bash
node --version   # e.g. v20.x.x
npm --version    # e.g. 10.x.x
```

### 2. Navigate to the project
```powershell
cd C:\Users\irtiz\.gemini\antigravity\scratch\portfolio
```

### 3. Install dependencies
```bash
npm install
```

### 4. Start the development server
```bash
npm run dev
```

Open your browser at **http://localhost:3000** 🎉

## ✏️ Personalisation

All content is centralised in **[`src/data/portfolioData.js`](./src/data/portfolioData.js)**. Edit the following:

| Export         | What to update                        |
|----------------|---------------------------------------|
| `personalInfo` | Name, email, phone, LinkedIn, GitHub  |
| `typingStrings`| Cycling role titles in hero           |
| `aboutText`    | Bio paragraphs                        |
| `stats`        | Stats counters                        |
| `skillCategories` | Skills with levels                |
| `experience`   | Work history                          |
| `projects`     | Projects with links                   |
| `education`    | Degree details                        |
| `certificates` | Certificates with PDF paths           |

### Update your resume
Replace `public/resume.pdf` with your actual resume PDF.

### Update social links
In `portfolioData.js`, update the `personalInfo` object:
```js
export const personalInfo = {
  linkedin: "https://linkedin.com/in/YOUR_USERNAME",
  github:   "https://github.com/YOUR_USERNAME",
  email:    "your@email.com",
  ...
};
```

## 🏗️ Build for Production

```bash
npm run build
```

The optimised output will be in the `dist/` folder.

Preview the production build locally:
```bash
npm run preview
```

## 🌐 Deployment

### Option 1: Vercel (Recommended — Free)

1. Push your project to a GitHub repository.
2. Go to [vercel.com](https://vercel.com) → **New Project** → Import your repo.
3. Vercel auto-detects Vite. Click **Deploy**.
4. Your site is live at `https://your-project.vercel.app` in ~1 minute!

**Or deploy via CLI:**
```bash
npm install -g vercel
vercel
```

### Option 2: GitHub Pages

1. Install the `gh-pages` package:
   ```bash
   npm install --save-dev gh-pages
   ```

2. Add to `package.json` scripts:
   ```json
   "predeploy": "npm run build",
   "deploy": "gh-pages -d dist"
   ```

3. In `vite.config.js`, set `base` to your repo name:
   ```js
   base: '/your-repo-name/'
   ```

4. Deploy:
   ```bash
   npm run deploy
   ```

Your site will be live at `https://YOUR_USERNAME.github.io/your-repo-name/`

### Option 3: Netlify

1. Push to GitHub.
2. Go to [netlify.com](https://netlify.com) → **Add new site** → **Import from Git**.
3. Build command: `npm run build`, Publish directory: `dist`
4. Click **Deploy**.

## 📋 Available Commands

| Command           | Description                    |
|-------------------|--------------------------------|
| `npm run dev`     | Start development server       |
| `npm run build`   | Build for production           |
| `npm run preview` | Preview production build       |
| `npm run lint`    | Run ESLint                     |

## 📄 License

MIT — free to use and modify for personal and commercial projects.

---

Built with ❤️ by **Irtiza Zain**
