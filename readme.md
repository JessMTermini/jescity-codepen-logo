# Unified Projects Master Workbench

Overall Project Timeline:

1. **Step 1:** Create a Local Directory Structure that mimics a real project.

2. **Step 2:** Use CSS Variables to unify the "stolen" colors.

3. **Step 3:** Component Work-Around: Use Iframes or Object Tags for high-risk interactivity (Three.js/Canvas).

4. **Step 4:** Create a Main Index to layout the pieces.

## Step 1: Multi-Project Structure Set-Up

```
/MASTER WORKBENCH (This Repo - JESCITY-CODEPEN-LOGO)
    /my-mockup-project 1 (jescity-docus-home-mockup)
        index.html
        theme.css  <-- Where you define projects theme primary/secondary colors
    /my-mockup-project 2
        index.html
        theme.css
    /assets    <-- Muti-Project Assets like images
    /components    <-- (Multi-Project) Finished Components
        card.html    <-- These html snippets encapsulate html and css on a component level
        button.html
        ....html
        /experimental    <-- Components currently being built or worked on
            /cards
                glass-card.html
                grad-glow-cards.html
                ...
            /logo
                logo-v1.html
                logo-v2.html
                ...
            /...
    readme.md
```

## Step 2: The "Global Palette" (CSS Variables)

To solve the "Cookie Cutter" color problem, you don't need a framework. You need a Central Intelligence for your colors.

Create a file called `theme.css`. This is where you store your "non-standard" soul. Instead of hex codes, you use names that describe the vibe.

```css
/* theme.css */
:root {
  --brand-glow: #ff0080;
  --glass-border: rgba(255, 255, 255, 0.1);
  --deep-space: #050505;
  --text-vibrant: #e2e8f0;
}
```

**The Win:** When you move to Tailwind later, you just tell Tailwind to look at these variables. You won't have to "re-map" anything.
