# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![Design screenshot](https://github.com/TheCoder-Rahul/fontend_mentor_four_card_feature_section/blob/main/project_screenshot.png)

### Links

- 👉 [Solution URL](https://github.com/TheCoder-Rahul/fontend_mentor_four_card_feature_section.git)
- 👉 [Live Site URL](https://thecoder-rahul.github.io/fontend_mentor_four_card_feature_section/)

## My process

### Built with

- 👉 **Markup:** Semantic HTML5 for better accessibility and SEO.
- 👉 **Styling:** CSS3 with Custom Properties (variables) for a maintainable color scheme, font-properties, and different sizes.
- 👉 **Layout:** Flexbox for centering the card and managing the internal alignment.
- 👉 **Workflow:** Mobile-first approach and Responsive Design using Media Queries.

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

To see how you can add code snippets, see below:

```html
<main>
  <h1>Reliable, efficient delivery</h1>
  <h2>Powered by Technology</h2>
  <p>Our Artificial Intelligence powered tools use millions of project data points to ensure that your project is successful</p>

  <section class="cards">
    <article class="card">
      <span></span>
      <h3>Supervisor</h3>
      <p>Monitors activity to identify project roadblocks</p>
      <img src="./images/icon-supervisor.svg" alt="Supervisor Icon">
    </article>

    <article class="card">
      <span></span>
      <h3>Team Builder</h3>
      <p>Scans our talent network to create the optimal team for your project</p>
      <img src="./images/icon-team-builder.svg" alt="Team Builder Icon">
    </article>

    <article class="card">
      <span></span>
      <h3>Karma</h3>
      <p>Regularly evaluates our talent to ensure quality</p>
      <img src="./images/icon-karma.svg" alt="Karma Icon">
    </article>

    <article class="card">
      <span></span>
      <h3>Calculator</h3>
      <p>Uses data from past projects to provide better delivery estimates</p>
      <img src="./images/icon-calculator.svg" alt="Calculator Icon">
    </article>
  </section>
</main>
```
```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
:root {
  --bold-font: 600;
  --light-font: 200;
  --normal-font: 400;
  --font-size: 0.9375rem;
  --red: hsl(0, 78%, 62%);
  --heading-font-size: 1.5rem;
  --blue: hsl(212, 86%, 64%);
  --cyan: hsl(180, 62%, 55%);
  --orange: hsl(34, 97%, 64%);
  --bg-color: hsl(0, 0%, 100%);
  --grey-400: hsl(212, 6%, 44%);
  --grey-500: hsl(234, 12%, 34%);
}
body {
  line-height: 1.5;
  text-align: center;
  color: var(--grey-500);
  font-size: var(--font-size);
  font-weight: var(--normal-font);
  background-color: var(--bg-color);
  font-family: 'Poppins', sans-serif;
}
main {
  padding: 3rem 2rem;
}
h1, h2 {
  font-size: var(--heading-font-size);
  font-weight: var(--light-font);
}
h2 {
  margin-bottom: 1rem;
  font-weight: var(--bold-font);
}
main > p {
  margin-bottom: 3rem;
}
.cards {
  gap: 2rem;
  display: flex;
  margin: 0 auto;
  flex-wrap: wrap;
  max-width: 1100px;
  justify-content: center;
}
.card {
  padding: 2rem;
  overflow: hidden;
  text-align: start;
  position: relative;
  border-radius: 0.5rem;
  background-color: var(--bg-color);
  box-shadow: 0px 0.5rem 1rem hsl(212, 40%, 90%);
}
.card:first-child span {
  background-color: var(--cyan);
}
.card:nth-child(2) span {
  background-color: var(--red);
}
.card:nth-child(3) span {
  background-color: var(--orange);
}
.card:last-child span {
  background-color: var(--blue);
}
.card span {
  content: '';
  inset: 0;
  width: 100%;
  height: 0.25rem;
  position: absolute;
}
.card h3 {
  margin-bottom: 0.5rem;
}
.card p {
  margin-bottom: 3rem;
  color: var(--grey-400);
  font-size: calc(var(--font-size) - 0.125rem);
}
.card img {
  display: block;
  margin-left: auto;
}
.attribution { font-size: 11px; text-align: center; position: absolute; bottom: 0.5rem; width: 100%; }
.attribution a { color: var(--grey-400); }

@media screen and (min-width: 768px) {
  :root {
    --heading-font-size: 2rem;
  }
  main {
    padding: 5rem 2rem;
  }
  main > p {
    max-width: 500px;
    margin: 0 auto 3.875rem;
  }
  .cards {
    gap: 2rem;
    display: grid;
    align-items: center;
    grid-template-rows: repeat(2, 1fr);
    grid-template-columns: repeat(3, 1fr);
  }
  .card:first-child {
    grid-row: 1 / span 2;
  }
  .card:nth-child(2) {
    grid-row: 1;
  }
  .card:nth-child(3) {
    grid-row: 2;
  }
  .card:last-child {
    grid-row: 1 / span 2;
  }
}
```

## Author

- 👉 GitHub - [TheCoder-Rahul](https://github.com/TheCoder-Rahul)
- 👉 Frontend Mentor - [@TheCoder-Rahul](https://www.frontendmentor.io/profile/TheCoder-Rahul)
- 👉 LinkedIn - [@Rahul Kumar](https://www.linkedin.com/in/rahul-the-developer/)