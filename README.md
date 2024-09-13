# Linus Chirchir's Personal Portfolio Website Repository

This repository contains the source code and configuration for my personal portfolio website, [linuschirchir.com](https://linuschirchir.com), created with Quarto, hosted on GitHub Pages, and deployed via GoDaddy.

![Website Preview](images/website_preview.png)

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Site Structure](#site-structure)
- [Customisation](#customisation)
- [Setting Up Your Custom Domain with GoDaddy](#setting-up-your-custom-domain-with-godaddy)
- [License](#license)

## Introduction

This repository is the foundation of my personal portfolio website, where I share insights and projects related to data science, artificial intelligence, machine learning, and health information systems. It includes sections such as my blog, professional CV, and various projects. The website is built using the [Quarto](https://quarto.org) framework, hosted on GitHub Pages, and uses a custom domain, [linuschirchir.com](https://linuschirchir.com), deployed via GoDaddy.

## Prerequisites

Before getting started, ensure you have the following installed:

- **Quarto**: The website is built using Quarto. You can download it from the [official site](https://quarto.org/).
- **Git**: To clone this repository and manage version control.
- **Web Browser**: To view the rendered site locally.

## Installation

To install and run the project locally, follow these steps:

1. Fork the repository:
   - Go to the repository page on GitHub: https://github.com/linuschirchir/linuschirchir.github.io.git
   - Click "Fork" in the top-right corner to copy the repository to your GitHub account.

2. Clone your forked repository to your local machine:
   ```bash
   git clone https://github.com/<your-GitHub-username>/linuschirchir.github.io.git
   cd linuschirchir.github.io
   ```

3. Install Quarto on your system. Follow the instructions on the [Quarto website](https://quarto.org/docs/get-started/).

4. Render the site locally:
   ```bash
   quarto render
   ```

5. Open the generated `_site/index.html` file in your browser to view the site.

## Site Structure

The main files and directories in this repository include:

- **_quarto.yml**: The primary configuration file for the site, including metadata, navigation setup, and layout configuration.
- **CNAME**: The custom domain configuration for GitHub Pages, pointing to [linuschirchir.com](https://linuschirchir.com).
- **about.qmd**: Quarto markdown file for the "About Me" page.
- **blog.qmd**: Section for blog posts, rendered using Quarto.
- **cv.qmd**: Contains my professional CV.
- **projects.qmd**: Details various data science and AI projects.
- **images/**: Directory containing images used across the site.
- **styles.css**: Custom styles for personalising the website’s appearance.
- **dark.scss & light.scss**: SCSS files to manage both light and dark themes.

## Customisation

You can customise various aspects of the site:

- **Theme**: Modify the `styles.css` or SCSS files to change the light and dark themes.
- **Content**: Update the Quarto markdown files (`.qmd`) to add or modify content such as blog posts, projects, or the CV.
- **Domain Setup**: The `CNAME` file points the website to the custom domain. If you are forking or adapting the repository, update the CNAME file to your own domain.

## Setting Up Custom Domain with GoDaddy

To set up custom domain for [linuschirchir.com](https://linuschirchir.com), I used GoDaddy as the domain registrar and GitHub Pages for hosting.

### Step 1: Set Up Your Quarto Site on GitHub Pages
Before connecting your domain, ensure that your Quarto site is deployed on GitHub Pages:

1. Push your Quarto site to a GitHub repository.
2. Go to the repository's settings.
3. Under the "Pages" section, set your source branch (either `main` or `gh-pages`) and choose the root directory or `/docs` as appropriate.

### Step 2: Purchase or Access Your Domain in GoDaddy
To use a custom domain, you'll need one registered with GoDaddy. If you haven't done this yet, you can purchase a domain through GoDaddy.

### Step 3: Update Your GitHub Repository for the Custom Domain
Link your domain to GitHub Pages:

1. In your GitHub repository, create a `CNAME` file at the root level (if it doesn’t already exist).
2. Inside the `CNAME` file, add your domain name (e.g., `www.linuschirchir.com`).
3. Commit and push the file to your repository.

### Step 4: Configure DNS Settings in GoDaddy
To point your domain to GitHub Pages:

1. Log in to your GoDaddy account.
2. In "My Products," find the domain you want to use.
3. Click "DNS" next to your domain to access DNS Management.
4. Set the following DNS records:
   - **A Record**: Point to these GitHub Pages IP addresses:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - **CNAME Record**: Point `www` to `<username>.github.io` (replace `<username>` with your GitHub username).

### Step 5: Wait for DNS Propagation
The DNS changes may take a few minutes to several hours to propagate fully.

### Step 6: Verify Your Custom Domain on GitHub
Once the DNS is propagated, go back to your GitHub repository settings. In the "Pages" section, confirm that your custom domain is correctly set. GitHub will also handle the SSL certificate for HTTPS automatically.

At this point, your Quarto website should be live and accessible at [linuschirchir.com](https://linuschirchir.com).

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute it as long as proper attribution is provided. See the `LICENSE` file for more information.

---

Happy browsing!  
**Linus Chirchir**  
[Visit My Website](https://linuschirchir.com)
