# Day 03 – CSS Styling and Box Model

## 🎯 Objective

Understand how layout works at a low level using only raw CSS. No framework, no utility classes. The goal is to control the box model with confidence and build a semantic layout that scales.

## 🧠 What I Learned

- The box model is not a theory — it's real space I can measure.
- `padding`, `margin`, and `border` behave differently based on flow and display mode.
- Default browser styles are ugly and inconsistent — normalize or reset is a must.
- Grids and flexbox aren't magic. They’re just rules I give to the browser.
- Writing CSS for layout is more about mental model than syntax.

## 🛠️ What I Built

- Clean HTML layout from Day 2, now with visual structure.
- Header, main content, and footer styled with spacing, hierarchy, and proper box sizing.
- `section` blocks styled as professional “cards” using flexbox/grid — no div soup.
- All styling lives in `styles.css`. HTML and CSS fully separated.

## 💡 Notes

- I tested layout in Firefox and Chromium manually — no tools yet.
- Avoided inline styles and `!important`.
- The CSS still needs polish. Right now, it’s functional, not beautiful — and that’s fine.
- I kept it raw to really “feel” how CSS behaves before using frameworks like Tailwind or component libs.

## 📌 Commit Summary

- `index.html` uses real structure, not div-based mockups.
- `styles.css` includes core layout rules: spacing, grid, card styling, and responsive breakpoints.
- No JS. No animation. Just layout and box behavior.

## ✅ Next

Refine visual design. Learn layout systems (12-column, spacing tokens, rem/em, etc).  
Prepare for upcoming modules: CSS architecture, design systems, and React-based layouting.

---
