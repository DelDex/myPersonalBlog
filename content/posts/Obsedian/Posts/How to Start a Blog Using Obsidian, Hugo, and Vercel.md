---
title: How to Start a Blog Using Obsidian, Hugo, and Vercel
date: 2024-12-03
draft: false
tags: 
  - tag1
  - tag2
---


Are you looking for a streamlined, cost-effective way to start your blog? Combining **Obsidian** for content creation, **Hugo** for static site generation, and **Vercel** for hosting gives you a powerful stack to create and manage a professional-looking website. This guide walks you through the process step-by-step.

Why This Stack?

- **Obsidian**: A markdown-based note-taking tool with a clean, distraction-free interface perfect for writing and managing content.
- **Hugo**: A fast and flexible static site generator that turns markdown files into beautifully designed web pages.
- **Vercel**: A free hosting platform with automated deployments and a global CDN for fast loading times.

---

## Step 1: Write Your Content in Obsidian

### Set Up Obsidian for Blogging

1. **Install Obsidian**: Download and install [Obsidian](https://obsidian.md/) on your computer.
2. **Create a Vault**: Set up a new vault for your blog content.
3. **Organize Your Files**:
    - Create a folder for blog posts (e.g., `content/posts`).
    - Use markdown files (`.md`) for each blog post, naming them appropriately (e.g., `my-first-post.md`).

### Write Your First Post

Start drafting in markdown:

markdown

Copy code

`--- title: "My First Blog Post" date: 2024-12-03 draft: false ---  Welcome to my blog! This is my first post. Stay tuned for more content!`

The `---` block is the **front matter** required by Hugo to recognize metadata like the title and date.

---

## Step 2: Build Your Website with Hugo

### Install Hugo

1. **Download Hugo**: Install Hugo from Hugo’s website.
2. **Create a New Site**:
    
    bash
    
    Copy code
    
    `hugo new site my-blog cd my-blog`
    
3. **Choose a Theme**: Hugo offers many themes. Browse Hugo Themes and pick one you like. For example:
    
    bash
    
    Copy code
    
    `git init git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke`
    
4. **Update the Configuration**: Edit the `config.toml` file to set your site’s title, theme, and other options:
    
    toml
    
    Copy code
    
    `baseURL = "https://your-blog.vercel.app/" languageCode = "en-us" title = "My Blog" theme = "ananke"`
    

### Add Your Content

Copy your markdown files from Obsidian into the `content/posts` directory of your Hugo site.

### Build the Site

Generate the static files:

bash

Copy code

`hugo`

The output is saved in the `public/` directory.

---

## Step 3: Deploy Your Site on Vercel

### Set Up Vercel

1. **Sign Up for Vercel**: Create a free account at [vercel.com](https://vercel.com/).
2. **Install the Vercel CLI**:
    
    bash
    
    Copy code
    
    `npm install -g vercel`
    
3. **Link Your Project**: Navigate to your Hugo site directory and deploy:
    
    bash
    
    Copy code
    
    `vercel`
    
    Follow the prompts to configure the deployment.

### Configure Hugo for Automatic Deployments

1. Push your Hugo site to a Git repository (e.g., on GitHub):
    
    bash
    
    Copy code
    
    `git add . git commit -m "Initial commit" git push origin main`


![](/images/pexels-singkham-178541-1108572.jpg)

