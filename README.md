# Hugo Blog Awesome GitHub Pages Deployment

This repository contains a starter setup for deploying a Hugo static site using the [`hugo-blog-awesome`](https://github.com/janraasch/hugo-blog-awesome) theme. The site is automatically deployed to GitHub Pages using a GitHub Actions workflow.

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
```

### 2. Install Hugo

Follow the [official Hugo installation guide](https://gohugo.io/getting-started/installing/).

### 3. Add the Theme

```bash
git submodule add https://github.com/janraasch/hugo-blog-awesome.git themes/hugo-blog-awesome
```

Update your `config.toml`:

```toml
theme = "hugo-blog-awesome"
```

### 4. Run Locally

```bash
hugo server -D
```

Visit [http://localhost:1313](http://localhost:1313) to view your site.

## Deploying to GitHub Pages

- Go to **Settings > Pages** in your GitHub repository.
- Setup the deployment to use the github workflow
- The workflow defintion file is present under `.github/workflows/hugo.yml`
- Edit your content in the `content/` directory.
- Update configuration in `config.toml`.

## References

- [Hugo Documentation](https://gohugo.io/documentation/)
- [hugo-blog-awesome Theme](https://github.com/janraasch/hugo-blog-awesome)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)