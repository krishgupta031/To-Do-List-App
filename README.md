# ⚒️ TASKFORGE

> *Forge your day, one task at a time.*

A sleek, dark-themed to-do list app built with pure HTML, CSS, and JavaScript — no frameworks, no dependencies, just vibes and productivity.

---

## ✨ Features

### 🎨 Visual Design
- **Animated background** — drifting glowing orbs with a subtle grid overlay create depth and atmosphere
- **Gradient logo** — color-shifting title animation using `background-clip: text`
- **Priority-coded task borders** — each task card shows a colored left-border accent:
  - 🔴 Red = High priority
  - 🟡 Gold = Medium priority
  - 🟢 Teal = Low priority
- **Confetti burst** — particle explosion fires from the checkbox when you complete a task
- **Smooth animations** — tasks slide in on creation and fade out on deletion

### ⚙️ Functionality
- **Add tasks** with a text input + priority selector (High / Medium / Low)
- **Complete tasks** by clicking the animated checkbox
- **Delete tasks** with the hover-reveal × button
- **Filter view** by: All · Active · Done · 🔥 High Priority
- **Circular progress ring** showing your completion percentage at a glance
- **Live stats bar** tracking Total, Done, and Remaining counts
- **Clear completed** button appears automatically when done tasks exist
- **LocalStorage persistence** — your tasks survive page refreshes

---

## 🚀 Getting Started

No build step. No install. Just open the file.

```bash
# Clone or download the file, then:
open todo.html
```

Or drag `todo.html` into any browser window.

---

## 📁 File Structure

```
taskforge/
└── todo.html      # Single self-contained file — all HTML, CSS & JS included
└── README.md      # This file
```

Everything lives in one file — styles, logic, and markup — making it trivially easy to deploy, share, or embed.

---

## 🛠️ Tech Stack

| Layer      | Choice                        |
|------------|-------------------------------|
| Markup     | Semantic HTML5                |
| Styling    | Vanilla CSS (custom properties, keyframe animations, CSS Grid/Flexbox) |
| Logic      | Vanilla JavaScript (ES6+)     |
| Fonts      | Google Fonts — *Bebas Neue* + *DM Sans* |
| Storage    | `localStorage` API            |
| Icons      | Unicode emoji + inline SVG    |

Zero npm packages. Zero build tools. Zero dependencies beyond a Google Fonts CDN call.

---

## 🎮 Usage

| Action | How |
|---|---|
| Add a task | Type in the input field → press `Enter` or click **ADD** |
| Set priority | Use the ⚡/🔥/🌿 dropdown before adding |
| Complete a task | Click the checkbox on the left |
| Delete a task | Hover the card → click the **×** button |
| Filter tasks | Click a filter pill: All / Active / Done / 🔥 High |
| Clear done tasks | Click the dashed **Clear completed tasks** button at the bottom |

---

## 🎨 Customization

All colors are defined as CSS custom properties at the top of the `<style>` block:

```css
:root {
  --bg:      #0a0a0f;   /* Page background */
  --surface: #111118;   /* Input / stats surface */
  --card:    #16161f;   /* Task card background */
  --border:  #2a2a3a;   /* Borders */
  --accent:  #ff4d6d;   /* Red — high priority / logo */
  --accent2: #7b61ff;   /* Purple — focus states / active filter */
  --accent3: #00d4aa;   /* Teal — done / low priority / progress ring */
  --text:    #e8e8f0;   /* Primary text */
  --muted:   #5a5a78;   /* Secondary / placeholder text */
}
```

Swap any of these values to re-theme the entire app instantly.

---

## 📸 Highlights

- **No frameworks** — everything in ~670 lines of clean, readable code
- **Single file** — copy one `.html` file anywhere and it just works
- **Persistent** — tasks are saved to `localStorage` automatically on every change
- **Responsive** — fluid layout works from 320px mobile up to wide desktop
- **Accessible** — keyboard-friendly input (`Enter` to add), clear focus states

---

## 📄 License

MIT — do whatever you want with it.
