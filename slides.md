---
theme: penguin
colorSchema: light
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# page transition
transition: slide-left
# use UnoCSS
css: unocss
hideInToc: true
layout: intro
---

<style>
   :root {
      --slidev-controls-foreground: black !important;
      --slidev-slide-container-background: transparent !important;
    }
</style>
# How to Build a Web App Using React

Learn how to build an interactive blog using React. 


---
layout: default
hideInToc: true
---

# What you will **learn** today


<Toc maxDepth="1" ></Toc>

---

# 2min Webdev Review

### For this workshop, I'll assume you know the following:

- HTML
  ```html
  <div class="nice-heading">
    <p>Hello ADI!</p>
  </div>
  ```

- CSS
  ```css
  .nice-heading {
    font-weight: bold;
  }
  ```

---
hideInToc: true
---

# 2min Webdev Review

### For this workshop, I'll assume you know the following:

- How to open the terminal
  ```bash
  node --version
  git clone https://github.com/anthony-zhou/react-blog-workshop
  ```
---

# What is React?

### React is:

- An open-source JavaScript library for building user interfaces.
- Maintained by Facebook and a large open-source community
- Often used in hackathons with MERN stack
  - MongoDB
  - Express
  - React
  - Node

---
level: 2
---

<div className="grid grid-cols-4 gap-5xl w-2/3 mx-auto my-15">
<img src="/react-companies-1.png" />
<img src="/react-companies-2.png" />
<img src="/react-companies-3.png" />
<img src="/react-companies-4.png" />
<img src="/react-companies-5.png" />
<img src="/react-companies-6.png" />
<img src="/react-companies-7.png" />
<img src="/react-companies-8.png" />
</div>

## Companies that use React

---
level: 2
---

# Advantages of React

### Compared to base HTML/CSS:

- Component-Based
- Package ecosystem
- Declarative

### Compared to other frameworks (Svelte, Vue, Angular):

- Easy to learn
- More robust package ecosystem
- Bigger developer community
- Cross-platform

---
level: 2
---

# What is Next.js?

### Next.js is:

- An open-source JavaScript library that enhances the capabilities of React
- Used with React in production applications (Audible, Twitch, Notion, Nike, etc.)
- A package that provides built-in optimizations, server-side rendering, and API routes for React.

### Why do we use Next.js?

- Basic React is slow
- Basic React has bad SEO

---
level: 2
---

# Sample React + Next.js Code

<a href="https://stackblitz.com/edit/nextjs-html-demo?file=pages/index.js">
Demo: HTML vs. Next.js
</a>


---
layout: center
---

# Let's build an app!

---
level: 2
title: "Task Outline"
---

# Here's what we'll do:

1. Create an empty project using Next.js, TypeScript, and TailwindCSS and set up a blog layout
2. Make it look pretty!
3. Load blog articles from Markdown files
4. Add bells and whistles

---
level: 2
---

# Set up the project

1. First, clone the template from GitHub
```bash
git clone https://github.com/anthony-zhou/next-starter
cd next-starter
yarn install
yarn dev
```

2. Next, create a file `data.ts` and add some dummy data.
  
3. Load the data into your `Home` component

---
level: 2
---

# Make it look pretty

- Let's consult [ChatGPT](https://chat.openai.com)

![ChatGPT screenshot](/chatgpt.png)

---
level: 2
---

# Load blog articles from Markdown

### First, let's load the posts on the homepage:

1. Install the required dependencies
```bash
yarn add remark remark-html gray-matter
```

2. Create some posts in `/posts`
   
3. Write a function to fetch the list of posts in `lib/posts.ts`
   
4. Use `getStaticProps()` to load and display the blog posts.

---
level: 2
---

# Load blog articles from Markdown

### Now, let's show the markdown for an individual page

1. Make a new page `pages/posts/[id].tsx`
2. Write a function to fetch an individual post in `lib/posts.ts`
3. Call the function from your new page
4. Link to the `[id].tsx` page from `Home`
5. Install `@tailwindcss/typography`

---

# Bells and whistles

Now that we have a simple blog ready to go, let's make it interactive! Here are some options:

- Add a counter
- Add a button that makes it rain confetti
- Add coffeeshop music
- ... whatever you can think of!


---

# Wrapping Up

More resources:

- [Next.js docs](https://nextjs.org/docs)
- [React.js docs](https://react.dev/learn)
- [TailwindCSS docs](https://v2.tailwindcss.com/docs)

You can reach me at az2681@columbia.edu