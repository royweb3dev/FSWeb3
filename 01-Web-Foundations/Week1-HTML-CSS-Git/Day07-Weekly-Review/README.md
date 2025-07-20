# Week 1 Review: Building the Foundation

## A Quick Retrospective

This first week was all about laying the groundwork. We went from an empty directory to a structured, styled, and version-controlled portfolio. It felt like a sprint, moving from abstract concepts like semantic HTML to tangible results with CSS layouts and components. The main focus wasn't just on _what_ to write, but _why_ we write it a certain way.

Here’s a breakdown of what truly clicked for me this week.

### 1. On Semantic HTML: It's Not for Me, It's for the Machines

**Question:** Why is `<nav>` better than `<div class="nav">`?

**My Take:** For a long time, I thought semantic HTML was just about making code "cleaner" for other developers. That's true, but it's a minor benefit. The real "aha!" moment was realizing I'm writing code for two audiences: humans and machines.

Using `<nav>` gives a clear signal to search engines like Google ("Hey, this is the main navigation, these links are important!") and, crucially, to screen readers used by visually impaired users. A screen reader can announce, "You are in the navigation section," allowing a user to easily skip to the main content. A `<div>` is just a generic box; it offers no context. So, using `<nav>` isn't just a best practice—it's a foundational step for accessibility and SEO.

### 2. On CSS Layouts: Choosing the Right Tool for the Job

**Question:** Flexbox vs. Grid - when to use which?

**My Take:** This was the biggest source of confusion, but now it's becoming clearer. It boils down to one dimension vs. two dimensions.

**Flexbox is my go-to for components.** It's perfect for arranging items in a single line, either horizontally or vertically. A classic example is a button with an icon and text. I just need to align those two things next to each other and center them vertically. Flexbox (`display: flex`, `align-items: center`, `gap`) handles this perfectly with minimal code. Our portfolio header's sub-row, where I needed to push the subtitle and the nav to opposite ends, was another perfect use case for `justify-content: space-between`.

**Grid, on the other hand, is for the overall page layout.** When I needed to arrange the main sections of my portfolio—the cards for Skills, Projects, etc.—into a responsive, multi-column layout, Grid was the obvious choice. It let me define a "scaffolding" for the page and place items precisely within it, controlling both rows and columns at the same time. Trying to build that card layout with Flexbox would have been a nightmare of nested divs.

The rule of thumb I'm adopting: **Use Grid for the page's skeleton, and Flexbox for the organs inside that skeleton.**

### 3. On Git Branching: The "Safety Net" for Development

**Question:** Why create a branch instead of working directly on `main`?

**My Take:** Working directly on `main` feels like performing surgery on a patient's heart while they're awake and running a marathon. It's incredibly risky.

Creating a branch (`git switch -c new-feature`) is like moving the patient to a sterile operating room. It creates an isolated, safe copy of the project where I can experiment, break things, and make commits without any fear of damaging the stable, working version (`main`).

Once the feature is complete and tested in that isolated environment, I can confidently "merge" it back. If I mess up completely, I can just discard the branch, and the `main` branch is never harmed. It's a fundamental safety net that makes collaborative work possible and keeps the main codebase reliable at all times. After the repository cleanup we did, this concept is now crystal clear.
