# Day 06: Thinking in Components - The Reusable Button

## Today's Mission

The goal today wasn't just to style a button. It was to shift my mindset from "styling a page" to "building a system." I focused on creating a reusable, consistent, and maintainable button component—my first real piece of a personal design system.

## Key Concept: The Power of Modifier Classes

The core idea I practiced today was using a base class (`.btn`) and tacking on a "modifier" class (`.btn--secondary`) to create variations.

Here’s my takeaway on why this is so powerful:

- **DRY (Don't Repeat Yourself):** The `.btn` class holds all the common styles—padding, font size, border radius, transition effects. I only had to write that code once.
- **Maintainability:** If I decide to change the default padding on all my buttons tomorrow, I only have to change it in one place: the `.btn` rule. Every button on the site will instantly update.
- **Clarity and Intent:** When I look at my HTML (`<a class="btn btn--secondary">`), it's immediately obvious what it is. It's a `btn`, and its specific style is `secondary`. The code documents itself.

This feels like a much more professional and scalable way to write CSS compared to creating one-off styles for everything.

## In-Practice: Flexbox for Perfect Alignment

A small but crucial part of this task was aligning the icon and text inside the button. This was a perfect, real-world use case for Flexbox:

1.  `display: inline-flex` on the `.btn` class turned it into a flex container without making it a block-level element.
2.  `align-items: center` perfectly centered the icon and text vertically.
3.  `gap: 0.75rem` provided clean, consistent spacing between them.

It's amazing how three lines of Flexbox code can solve alignment problems that used to be incredibly frustrating.

## Proof of Work & Integration

After building the button components in a separate "lab" environment, I integrated the final CSS into my main `styles.css` file. I then applied the `.btn` class to the "Commit Evidence" links in my portfolio.

- **See the result:** [Link to the specific commit on GitHub](https://github.com/royweb3dev/FSWeb3/commit/your-commit-hash-here) _(You'll need to replace this with your actual commit hash.)_
- **Screenshot of the final buttons in the portfolio:**
  ![Proof of Work section with new buttons](path/to/your/screenshot.png) _(You'll need to add your screenshot to the Day06 folder and link it here.)_

## What's Next

This was the last day of new material for the week. Tomorrow is a review day, where I'll solidify these foundational concepts of HTML structure, Git workflow, and CSS layouts before heading into week two.
