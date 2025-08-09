# Hugo Blog

This repository contains the source code for a personal or project blog built using [Hugo](https://gohugo.io/), a fast and modern static site generator.

## Features

* **Blazing Fast:** Built with Hugo, this site is compiled into static HTML, making it incredibly fast and secure.

* **Simple Content Management:** All content is written in Markdown, which is easy to read and write.

* **Version Controlled:** The entire site, including content, is managed with Git.

* **Responsive Design:** The theme used is fully responsive and looks great on all devices.

## Getting Started

Follow these steps to get a local copy of the project up and running.

### Prerequisites

* **Git:** To clone the repository.

* **Hugo:** You must have Hugo installed on your system. You can find installation instructions on the [official Hugo website](https://gohugo.io/getting-started/installing/).

### Installation

1.  **Clone the repository:**

    ```
    git clone [git@github.com:black-sheep-meedia/bsm-blog.git](git@github.com:black-sheep-meedia/bsm-blog.git).
    cd bsm-blog
    ```

2.  **Initialize the theme (if it's a submodule):**

    ```
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

* **`config.toml`**: The main configuration file for the entire site.

## Adding Content

To add a new blog post, use the following command:

```
hugo new posts/my-new-post.md
```

This will create a new Markdown file with a pre-populated front matter in the `content/posts/` directory.

## Theme

This site uses the **\[Ananke]** theme. You can find more information and documentation for the theme at [https://ananke-theme.netlify.app/](https://ananke-theme.netlify.app/).

