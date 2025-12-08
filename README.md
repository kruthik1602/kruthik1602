<h1 align="center">👋 Hey, I'm Kruthik Reddy Theepireddy</h1>

<p align="center">
  Data Analyst & Data Engineer · Building AI-first analytics products
</p>

---

<p align="center">
  <!-- Profile Views -->
  <img src="https://komarev.com/ghpvc/?username=kruthik1602&label=Profile%20Views&style=for-the-badge" alt="profile views" />
  
  <!-- Followers -->
  <a href="https://github.com/kruthik1602?tab=followers">
    <img src="https://img.shields.io/github/followers/kruthik1602?style=for-the-badge&logo=github" alt="GitHub followers" />
  </a>
  
  <!-- Portfolio Badge -->
  <a href="https://your-portfolio-url.com">
    <img src="https://img.shields.io/badge/Portfolio-Live-00ff88?style=for-the-badge&logo=google-chrome&logoColor=white" alt="portfolio" />
  </a>

  <!-- LinkedIn -->
  <a href="https://www.linkedin.com/in/your-linkedin-id">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="linkedin" />
  </a>
  
  <!-- Resume -->
  <a href="resume.pdf">
    <img src="https://img.shields.io/badge/Resume-Download-FFB300?style=for-the-badge&logo=readme&logoColor=white" alt="resume" />
  </a>
</p>

> 🔧 **Note:** Replace `kruthik1602`, `your-portfolio-url.com`, `your-linkedin-id`, and `your-resume-link.com` with your actual handles/links.

---

## 🧭 About Me

- 🎓 Data Analyst & Engineer with experience across **analytics, ETL, and BI**  
- 🧪 Focused on **AI-powered data products** – ETL automation, quality monitoring, pricing, and insight generation  
- 📊 Love taking messy real-world data → **clean pipelines, dashboards, and decision tools**  
- 🚀 Currently working on **shipping production-grade analytics tools** that look and feel like real startup products

---

## 🌀 Portfolio – Single Page Animated Website

This repo contains my **single-page, high-impact portfolio** built as a standalone `index.html` (all CSS & JS inlined), optimized for:

- Recruiters & hiring managers who want to **see real products in seconds**
- Fast deploy to **GitHub Pages / Vercel / Render / any static host**
- Clean structure: sections for **Hero → Experience → Skills → Projects → Before/After → Education → Contact**

### 🔗 Live Portfolio

- 🌐 **Live Site:** `https://your-portfolio-url.com`  
- 💾 **Single File Version:** `kruthik_portfolio_single_file.html` (all styles + JS embedded)

---

## 🎞️ Motion & Animation System

The portfolio leans heavily on **CSS, JS, and SVG-friendly animation patterns** to feel like a real product site, not a static CV.

### 1️⃣ Hero & Global Interactions

- **Staggered Hero Title Animation**  
  The main headline lines (`Build Data Solutions / like a startup / even if you aren't one`) animate in with:
  - Per-line staggered entrance
  - Smooth `transform + opacity` transitions
  - Initialized via `initHeroAnimation()` on `DOMContentLoaded`

- **Horizontal Marquee Strip**  
  A continuous marquee showing roles like `DATA ANALYST · DATA ENGINEER · PYTHON DEVELOPER · TABLEAU EXPERT · POWER BI PRO`:
  - Infinite `@keyframes scroll-left` animation
  - GPU-friendly transforms for smooth performance

- **Scroll Indicator (SVG-friendly)**  
  A vertical **scroll arrow line** under the hero:
  - CSS `@keyframes scroll-down` to move the line up/down and fade it in/out
  - Designed so it can be replaced with an **inline SVG arrow** without changing the logic

- **Fixed Section Counter**  
  A minimal `[ 01 / 07 ]` section counter on the right:
  - Updated by JS on scroll via `initSectionCounter()`
  - Highlights where you are in the page at all times

---

### 2️⃣ Scroll-Triggered Animations

The portfolio uses **IntersectionObserver** (no heavy libraries) to animate content as it comes into view:

- `.fade-in` elements:
  - Start at `opacity: 0` and `translateY(30px)`
  - When visible, transition to `opacity: 1` and `translateY(0)`
  - Used on cards, sections, content blocks across the site

- **Experience Cards & Project Cards**  
  Each card:
  - Fades & slides in when entering viewport
  - On hover, slightly **lifts** with a soft shadow and **accent glow** using `::before` pseudo-elements
  - Gives a subtle **3D-like feel** without WebGL

- **Before/After Comparison Section**  
  The “Before vs After using my tools” section:
  - LEFT column (“Before”) cards describe pain points (siloed data, manual reports, quality issues)
  - RIGHT column (“After”) cards describe AI-powered outcomes  
  Each card is animated via the same scroll/fade-in system for continuity.

---

### 3️⃣ Advanced Text & Metric Animations

The animation JS includes reusable utilities that can drive rich text + numeric effects:

- **Text Reveal Animation** (`initTextRevealAnimation`)  
  For any element with `data-reveal`:
  - JS splits text into **per-word spans**
  - Applies staggered `animation-delay` to each word
  - Supports **per-word reveal** (great for headings or quotes)

- **Number Counter Animation** (`animateCounter`)  
  For metric/achievement numbers (e.g., `30+ analytics solutions`, `1M+ records`):
  - Smooth `0 → target` count-up effect using `requestAnimationFrame`
  - Can be attached to KPIs like: projects shipped, datasets processed, etc.

You can hook these into future **SVG-based dashboards or logos** easily by:

- Binding `data-reveal` to `<text>` labels inside SVG  
- Using `animateCounter` to drive numeric `<text>` nodes in an SVG KPI panel

---

### 4️⃣ Parallax & Reduced Motion Support

- **Parallax Effects** (`initParallaxEffect`)  
  Elements with `[data-parallax]` respond to scroll:
  - Subtle background shifts to create **depth**
  - Designed to work with hero shapes, gradient blobs, or SVG illustrations

- **Accessibility – `prefers-reduced-motion`**  
  In `animations.css`:
  - If a user has **reduced motion** enabled:
    - Disables non-essential animations
    - Stops marquee and scroll arrow animations
    - Great for accessibility & performance

---

## 🧰 Tech Stack

### 🧠 Data & Analytics

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Snowflake-29B5E8?logo=snowflake&logoColor=white" />
  <img src="https://img.shields.io/badge/Alteryx-0078AA?logo=alteryx&logoColor=white" />
  <img src="https://img.shields.io/badge/ETL-Pipelines-00ff88" />
</p>

### 📊 BI & Visualization

<p>
  <img src="https://img.shields.io/badge/Tableau-E97627?logo=tableau&logoColor=white" />
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?logo=powerbi&logoColor=black" />
  <img src="https://img.shields.io/badge/Plotly-DARKBLUE?logo=plotly&logoColor=white" />
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white" />
</p>

### 🧱 Web & Infra

<p>
  <img src="https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white" />
  <img src="https://img.shields.io/badge/Render-00979D?logo=render&logoColor=white" />
</p>

---

## 🚀 Flagship Projects (from the Portfolio)

Each card on the portfolio page links to a **real, hosted project**:

### 1. AI AutoETL Pipeline Generator

> Upload raw datasets → get **ready-to-run ETL pipelines** (SQL + Python + YAML)

- Detects schema & data types
- Generates cleaning + transformation logic automatically
- Outputs DDL/DML for Postgres / MySQL / Snowflake
- Metadata store to track schema profiles & generated artifacts

### 2. AI Data Quality Monitor & Anomaly Detector

> Treats data quality like **production monitoring**

- Column-level quality checks (nulls, outliers, distribution shifts)
- Rule-based + ML-based anomaly detection
- Rich HTML/Streamlit reporting with flags and recommendations
- Great for “before data goes into dashboards” governance

### 3. AI Insights Dashboard (Automated Story Generator)

> Turns raw data into **dashboards + narratives**

- Detects dataset structure and domain
- Builds charts (time series, bar, correlation)
- Runs forecasting (Prophet / ARIMA) on time series
- Uses LLM to generate **human-readable commentary** on trends

### 4. Pricing Strategy Intelligence Tool

> Experiments with **pricing, elasticity, and risk**

- Upload experiments / pricing test data
- Simulates **“what if”** scenarios on price changes
- Combines elasticity, A/B numbers, and forecasted revenue
- LLM-powered narrative explaining **tradeoffs & risks**

---

## 📈 GitHub Analytics

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=kruthik1602&show_icons=true&theme=radical" alt="GitHub stats" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=kruthik1602&theme=radical" alt="GitHub streak" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=kruthik1602&layout=compact&theme=radical" alt="Top languages" />
</p>

> Again, swap `kruthik1602` with your actual GitHub username if different.

---

## 📬 Contact

- 💼 LinkedIn: [`linkedin.com/in/your-linkedin-id`](https://www.linkedin.com/in/your-linkedin-id)  
- 📧 Email: `yourname@email.com`  
- 🌐 Portfolio: [`your-portfolio-url.com`](https://your-portfolio-url.com)

If you’re hiring for **Data Analyst / Analytics Engineer / Data Engineer** roles and want someone who ships **real tools**, feel free to reach out.
