# Hatch Design Reference & UI System (Permanent Workspace Standard)

> **Core Aesthetic**: Hand-drawn zine meets pastel candy store on a warm cream canvas. Pure white cards, crisp 1px ink-black outlines, chunky serif headlines with hand-drawn mint highlight swashes, scattered pastel confetti dots, and a friendly mascot. NO drop shadows anywhere.

---

## 🎨 Color Palette & Roles

| Name | Hex | Role |
| :--- | :--- | :--- |
| **Cream Paper** | `#f5f4f0` | Page canvas & background — warm off-white that softens pastel accents. |
| **Pure White** | `#ffffff` | Elevated card surfaces and button layers (1 elevation above cream). |
| **Ink Black** | `#000000` | Dominant structural color: all 1px hairline borders, text, and outlines. |
| **Charcoal** | `#222222` | Body copy and secondary descriptions. |
| **Slate** | `#333333` | Nav text and subtle metadata labels. |
| **Mint Splash** | `#99ffcc` | **PRIMARY ACTION COLOR ONLY**: Filled CTA buttons, headline highlight swashes, active badges. |
| **Sky Pop** | `#7bbbff` | Decorative mascot, illustration strokes, secondary chip accents. |
| **Bubblegum** | `#ff99cc` | Confetti dots, headphones accent, playful chips. |
| **Peach Pop** | `#ffcc99` | Confetti dots, warm accent fills, category badges. |

---

## ✍️ Typography Guidelines

1. **Headlines (`DM Serif Display` / `Recoleta 700`)**:
   - High-contrast, chunky bold serif used for all major headlines and section titles.
   - Tight negative tracking (`-0.028em`).
   - Scales from 32px up to 92px+.
2. **Body & UI (`Inter` / `Lota Grotes Que Alt`)**:
   - Quiet, utilitarian grotesque at 18px body size with generous line height (`1.5–1.6`).
   - Font weight 700 for buttons and emphatic UI labels; 400 for paragraphs.
3. **Mint Highlight Swashes**:
   - An irregular organic brush/oval shape in `#99ffcc` placed behind 1–2 keywords per headline. Never swash the entire headline.

---

## 📐 Shapes, Elevation & Layout

- **ZERO Box Shadows**: Depth comes purely from the contrast between cream canvas (`#f5f4f0`), white cards (`#ffffff`), and 1px solid `#000000` borders. Never add `box-shadow`.
- **Card Border Radius**: Exactly `16px`.
- **In-Page Buttons**: `12px` border-radius, 1px solid `#000000` border, 18px bold text.
- **Persistent Nav CTA & Tag Chips**: Full `9999px` pill radius.
- **Confetti Dots**: 6–12px circles scattered asymmetrically in the 4 pastels (mint, sky, pink, peach).
- **Mascot**: Hand-drawn blue speech bubble with pink headphones and a winking face.
