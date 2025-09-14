# Black Sheep Meedia Blog

This repository contains the source code for the Black Sheep Meedia blog, built using [Hugo](https://gohugo.io/) with the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme. This blog showcases AI-powered editorial solutions and insights for modern media.

## Features

* **Blazing Fast:** Built with Hugo, this site is compiled into static HTML, making it incredibly fast and secure.

* **Modern Design:** Uses the PaperMod theme with dark/light mode, search functionality, and mobile responsiveness.

* **AI-Focused Content:** Dedicated to sharing insights on AI integration in editorial workflows.

* **Automated Deployment:** GitHub Actions automatically builds and deploys to GitHub Pages.

* **Scheduled Posts:** Daily builds ensure scheduled content is published automatically.

* **Slack Notifications:** Get notified of deployment status via Slack.

## Getting Started

Follow these steps to get a local copy of the project up and running.

### Prerequisites

* **Git:** To clone the repository.

* **Hugo:** You must have Hugo installed on your system. You can find installation instructions on the [official Hugo website](https://gohugo.io/getting-started/installing/).

### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/black-sheep-meedia/bsm-blog.git
    cd bsm-blog
    ```

2.  **Initialize the PaperMod theme submodule:**

    ```bash
    git submodule update --init --recursive
    ```

### Local Development

To see your site live as you work, run Hugo's built-in development server. This will watch for changes and rebuild the site automatically.

```
hugo server
```

Navigate to `http://localhost:1313` in your browser to view the site.

## Site Structure

The key directories in a Hugo project are:

* **`content/`**: All your content files (blog posts, pages) go here, organized by sections.

* **`themes/`**: This is where the site's theme lives.

* **`static/`**: Files placed here (like images, CSS, JavaScript) will be copied directly to the root of the generated site.

* **`hugo.toml`**: The main configuration file for the entire site.

* **`.github/workflows/`**: GitHub Actions workflow for automated deployment.

## Adding Content

To add a new blog post, use the following command:

```bash
hugo new posts/my-new-post.md
```

This will create a new Markdown file with a pre-populated front matter in the `content/posts/` directory.

## Deployment

The blog is automatically deployed to GitHub Pages using GitHub Actions:

- **Trigger**: Every push to the `main` branch
- **Schedule**: Daily at 6 AM UTC (for scheduled posts)
- **URL**: https://blog.blacksheepmeedia.com
- **Notifications**: Slack notifications for deployment status

## Theme

This site uses the **[PaperMod](https://github.com/adityatelange/hugo-PaperMod)** theme, which provides:

- Modern, clean design perfect for professional blogs
- Dark/light mode toggle
- Built-in search functionality
- Mobile responsive design
- SEO optimization
- Fast loading times

## Custom Domain

The blog is configured to use the custom domain `blog.blacksheepmeedia.com`. DNS configuration is required to point this domain to GitHub Pages.

## Scheduled Posts

To create scheduled posts, add a `publishDate` in the front matter:

```yaml
---
title: "Future Post"
date: 2024-01-15T10:00:00Z
publishDate: 2024-01-20T10:00:00Z
draft: false
---
```

The daily GitHub Actions workflow will automatically publish posts when their `publishDate` is reached.

