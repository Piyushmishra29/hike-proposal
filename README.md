# 🏔️ Hike Proposal

> *"Cutie, will you go on a hike with me?"* 🐻

A ridiculously over-engineered, interactive HTML page designed to ask someone very special on a hike. Built with vanilla HTML/CSS/JS, way too many emojis, and a "No" button that refuses to be clicked.

## ✨ Features

- 🌸 **Flower cursor trail** (desktop) — your mouse leaves a trail of blossoms
- 🏕️ **Emoji rain** (mobile) — hiking-themed emojis drift down the screen
- 🏃 **Dodging "No" button** — hover over it and it teleports away while begging for mercy
- 🎉 **Confetti explosion** — when she (inevitably) says Yes
- 💕 **Floating hearts** — because romance
- 🎒 **Responsive** — looks great on phone & desktop

## 🚀 Live Site

Deployed at: `https://indigo-frog-162979.hostingersite.com/`

## 🛠️ Tech Stack

- HTML5
- CSS3 (with `backdrop-filter` blur & keyframe animations)
- Vanilla JavaScript
- [canvas-confetti](https://github.com/catdad/canvas-confetti) for the celebration

## 📁 Files

```
.
├── index.html   # The entire app in one file
└── README.md    # You are here
```

## 💡 How it works

1. The page loads with a cute question and two buttons.
2. The **"No"** button is a moving target — it jumps to random spots, changes its text to increasingly desperate pleas, and ignores taps on mobile.
3. The **"Yes"** button triggers a full confetti + hearts celebration and reveals the final message.
4. There is no escape. Only hike.

## 🎨 Customize It!

This page works for **any** question — a date, a proposal, a road trip, a kinky invite, or just asking someone to be your player 2. Everything lives in `index.html` and is easy to tweak.

### Quick Customization Cheat Sheet

| What | Where to edit | Default |
|------|---------------|---------|
| **Browser tab title** | `<title>` | `I have a question for you...` |
| **Big question** | `.question` | `Cutie, will you go on a hike with me?` |
| **Character emoji** | `.character` | `🐻` |
| **Yes button text** | `#btnYes` | `Yes!` |
| **Footer text** | `.footer-text` | `Say Yes with caution` |
| **Celebration header** | `.celebration h1` | `Yayyyy!` |
| **Celebration message** | `.celebration p` | `Pack your bags, we're going hiking!` |
| **Color vibe** | `body { background: ... }` | Pink gradient |
| **Cursor trail emojis** | `trailFlowers` array | `['🌸', '🌷', '🌺', '🌼', '💮']` |
| **Mobile rain emojis** | `rainEmojis` array | Hiking themed |
| **No button excuses** | `noTexts` array | Begging & bribery |

### Change the Theme Colors

Look for the `background:` gradient on the `body` selector. Swap the hex codes to match your vibe:

```css
/* Example: Midnight purple */
background: linear-gradient(160deg, #1a0b2e 0%, #2d1b4e 50%, #4a1c6b 100%);
```

Then update the button and text colors to match. Search for `#d6336c` (the pink accent) and replace it with your own color.

### Change the Question

Find this line:
```html
<h2 class="question">Cutie, will you go on a hike with me?</h2>
```

Replace it with whatever you're asking:
```html
<h2 class="question">Babe, will you be my player 2 tonight? 🎮</h2>
```

### Change the Celebration

Find the `.celebration` div and rewrite it:
```html
<div class="celebration" id="celebration">
  <span class="big-emoji">🍕🍷</span>
  <h1>Let's go!</h1>
  <p>Date night is ON.<br><br>I'll bring the snacks 😏</p>
  <span class="big-emoji">🔥❤️</span>
</div>
```

### Change the "No" Button Excuses

Find the `noTexts` array and make it yours:
```javascript
const noTexts = ["No", "Are you sure?", "Really?", "Think again!", "Please? 🥺",
  "Don't do this...", "I'll bring wine! 🍷", "Pretty please? 🙏", "Just click Yes 😤"];
```

That's it. One file. No build step. Just edit, save, and deploy. Good luck! 😉

## 📝 License

Made with love for someone who deserves a mountain view. ❤️
