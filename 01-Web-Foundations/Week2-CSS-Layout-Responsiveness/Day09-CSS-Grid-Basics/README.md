# Day 09: Understanding the Grid System

## Today's Focus

The goal wasn't to learn new tricks, but to deeply understand a tool I'm already using: CSS Grid. I spent today breaking down the `grid-template-columns` and `gap` properties that power my portfolio's card layouts. The real learning came from playing [Grid Garden](https://cssgridgarden.com/), which helped build a solid mental model.

## Core Lesson: `fr` vs. `%` Units

The most important distinction I learned today is how grid columns handle space.

- **`%` (Percentage):** This unit is strict. If you set three columns to `33.3%`, they take up that percentage of the parent container. The `gap` between them is then **added on top**, which can cause overflow and horizontal scrollbars. It doesn't account for the space between items.

- **`fr` (Fractional Unit):** This unit is smarter. It represents a fraction of the **available space**. If you have three `1fr` columns and a `1.5rem` gap, the browser first subtracts the total gap space, then divides the remaining space into three equal fractions. This makes it inherently flexible and prevents overflow, which is why it's the modern standard for this kind of layout.

In short, `fr` accounts for the `gap`, while `%` does not.

## Proof of Work

I've added comments to my main `styles.css` file, explaining each Grid property I've used. This was a great way to solidify my own understanding.

- **See the commented code:** [Link to the commit on GitHub](https://github.com/royweb3dev/FSWeb3/commit/your-commit-hash-here) _(You'll need to add the actual commit hash.)_

**Next:** Comparing Grid with Flexbox to know when to use which.
