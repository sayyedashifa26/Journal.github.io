Glitch DIARIES 

> A beautifully animated personal journal web app for writing thoughts, experiences, lessons, and stories — in a distraction-free interface with OTP-protected writing access.

---

## Features

- 📝 Create, edit, and delete journal entries
- 🔐 Email OTP authentication — only you can write
- 🗂️ Category filters (Life, Work, Travel, Learning, Random)
- 🔍 Instant keyword search across all entries
- 📊 Writing statistics — total entries, words written & daily streak
- 🎨 Animated 3D book & pen hero with floating particles and stars
- 📱 Fully responsive — mobile, tablet & desktop
- 💾 Local storage persistence — no backend required
- ✨ Dancing Script calligraphy font with ice blue accent theme

---

## Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Structure and markup |
| CSS3 | Animations, custom properties, 3D transforms |
| Vanilla JavaScript (ES6+) | App logic, OTP flow, storage |
| Local Storage API | Persistent journal entries |
| EmailJS | OTP email delivery for write protection |
| Google Fonts | Dancing Script, DM Sans |

---

## Project Structure

```
journal.github.io/
├── index.html       ← Entire app — single self-contained file
├── README.md        ← You are here
└── LICENSE          ← MIT License
```

> The entire app lives in **one HTML file** — HTML structure, CSS in a `<style>` block, and JavaScript in a `<script>` block. No frameworks, no build tools, no `node_modules`.

---

## 📦 Everything in One File

This entire project — **HTML, CSS, JavaScript, animations, OTP logic, storage, fonts and UI** — is packaged inside a single `index.html` file.

```
index.html
├── <head>        → fonts, meta tags
├── <style>       → all CSS (animations, 3D effects, responsive layout, variables)
├── <body>        → all HTML (header, hero, book animation, cards, modals)
└── <script>      → all JavaScript (storage, OTP, filters, search, stats)
```

There is **no** separate:
- ❌ `.css` file
- ❌ `.js` file
- ❌ `node_modules`
- ❌ `package.json`
- ❌ build step or bundler

Just download `index.html` and it works. That's it.

---

## OTP Authentication

Writing access is protected by a **one-time password** system powered by EmailJS.

**How it works:**
1. Anyone can visit the blog and read all entries freely
2. Clicking **+ New Entry** or **Edit** triggers the OTP flow
3. A 6-digit code is sent instantly to the owner's Gmail
4. Enter the correct code within 5 minutes to unlock writing
5. Wrong code → inputs flash red
6. Resend available after 30 seconds

> ⚠️ OTP only works on the live GitHub Pages URL — not when opening `index.html` locally.

---

## How to Run

### View live
Visit: [https://sayyedashifa26.github.io/journal.github.io/](https://sayyedashifa26.github.io/Journal.github.io/)

### Clone and deploy yourself

```bash
git clone https://github.com/sayyedashifa26/journal.github.io.git
cd journal.github.io
```

Then open `index.html` in your browser to view (note: OTP requires a live hosted URL).

---

## Data Storage

Entries are stored in the browser using the **Local Storage API**. No account or server required.

```
Storage Key: glitch-diaries-posts
```

> ⚠️ Clearing browser data will remove all entries. For permanent storage, consider adding cloud sync in a future version.

---

## Future Improvements

- [ ] Cloud sync (Firebase / Supabase)
- [ ] Markdown support in entries
- [ ] Dark / Light theme toggle
- [ ] Export entries as PDF or JSON
- [ ] Tags and mood tracking
- [ ] Monthly archive view
- [ ] Share individual entry as link

---

## License

MIT License — free to use, fork and modify.

---

## Author

Built with creativity and curiosity ✦ by **Sayyeda Shifa**

