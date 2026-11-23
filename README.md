# Ankur Gupta - Video Editor Portfolio

A clean, modern, fully responsive, and cinematic portfolio website designed for freelance video editors.

## 🚀 Quick Start
Double-click `index.html` to open it in any web browser (Chrome, Safari, Firefox, Edge). No build step, Node.js, or local web server required!

---

## 🎨 Customizing Content (The CONFIG Object)

All dynamic text, projects, services, testimonials, pricing, and video links can be updated directly inside the **`CONFIG`** object located in `index.html` around line 2878:

```javascript
const CONFIG = {
  profile: {
    name: "Ankur Gupta",
    role: "Freelance Video Editor & Motion Designer",
    tagline: "I turn raw footage into stories people remember",
    email: "ankurgupta13579@gmail.com",
    phone: "+91 8887964050",
    whatsapp: "918887964050",
    ...
  },
  ...
}
```

### 1. Replacing Featured Showreel
Change the values under `featuredShowreel`:
- `videoUrl`: Direct `.mp4` URL or YouTube/Vimeo embed URL (e.g. `https://www.youtube.com/embed/YOUR_ID`).
- `posterUrl`: Image URL or path to your local screenshot (e.g. `assets/showreel-poster.jpg`).

### 2. Adding / Updating Portfolio Projects
Add or edit project objects in `CONFIG.projects`:
```javascript
{
  id: 1,
  title: "Your Project Title",
  category: "youtube", // Options: 'youtube' | 'reels' | 'wedding' | 'corporate' | 'motion'
  categoryLabel: "YouTube",
  client: "Client Name",
  views: "1.2M Views",
  posterUrl: "https://your-image-url.com",
  videoUrl: "https://your-video-url.com/clip.mp4",
  description: "Short description of what you edited.",
  software: ["Premiere Pro", "After Effects"]
}
```

### 3. Updating Stats & Software Bars
- **Stat numbers** (Years, Projects, Clients, Views) are set in the HTML under `#stats-counter-row` using `data-target="20"`.
- **Software skill percentages** are set in the HTML under `.skills-box` using `data-progress="95%"`.

### 4. Customizing Colors
In `index.html` in the `<style>` block:
- **Accent Color**: Change `--accent: #7c5cff;` (Electric Violet) to your preferred accent (e.g., `#00f2fe` for neon cyan, `#ff3366` for crimson, `#10b981` for emerald).
- **Background**: Change `--bg-base: #0b0b0f;` to adjust the dark theme tone.

---

## 🌐 Free Hosting Guide

### Option 1: Netlify Drop (Fastest - 30 seconds)
1. Go to [https://app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag and drop the `portfolio` folder containing `index.html`.
3. Your site is live instantly with an SSL certificate and custom subdomain!

### Option 2: GitHub Pages (Recommended for Developers)
1. Create a new GitHub repository named `portfolio` or `<your-username>.github.io`.
2. Push your `index.html` file to the `main` branch.
3. Go to **Settings** > **Pages** > Select `Deploy from a branch` > Choose `main` / `root` > Click **Save**.
4. Your website will be live at `https://<your-username>.github.io/portfolio/`.

### Option 3: Vercel
1. Install Vercel CLI (`npm i -g vercel`) or sign in at [vercel.com](https://vercel.com).
2. Connect your GitHub repository or drag-and-drop the directory.
3. Choose the default settings and hit **Deploy**.
