# Tom Griffin - Hugo Tufte Theme Site

Site built with the [hugo-tufte](https://github.com/loikein/hugo-tufte) theme.

## Quick Start

### Running the Local Server

```bash
hugo server --buildDrafts --disableFastRender
```

After starting, open your browser at `http://localhost:1313/`

### Creating a New Post

```bash
hugo new posts/post-name.md
```

### Building for Production

```bash
hugo
```

Generated files will be in the `public/` folder.

## GitHub Pages Deployment

### Initial Setup

1. **Update baseURL in `config.yaml`**:
   - Go to your repository on GitHub → Settings → Pages
   - Find your site URL (e.g., `https://username.github.io/repo-name/`)
   - Update `baseURL` in `config.yaml` to match exactly

2. **Enable GitHub Pages**:
   - Go to repository **Settings** → **Pages**
   - Under **Source**, select **GitHub Actions**
   - (Don't select a branch - GitHub Actions will handle deployment)

3. **Push to GitHub**:
   - Commit and push all files to the `main` branch
   - GitHub Actions will automatically build and deploy
   - Check the **Actions** tab to see the deployment progress

### Finding Your Site URL

Your site will be available at:
- **Project site**: `https://YOUR_USERNAME.github.io/REPO_NAME/`
- **User site**: `https://YOUR_USERNAME.github.io/` (if repo is named `username.github.io`)

### After Deployment

- Wait 1-2 minutes for the first deployment
- Your site will be live at the URL shown in Settings → Pages
- Future pushes to `main` will automatically trigger new deployments

## Project Structure

- `config.yaml` - site configuration
- `content/` - site content (posts, pages)
- `themes/hugo-tufte/` - Hugo Tufte theme
- `static/` - static files (CSS, JS, images)
- `.github/workflows/` - GitHub Actions workflows

## Configuration

Main parameters are configured in the `config.yaml` file:

- `title` - site title
- `params.subtitle` - subtitle
- `params.math` - enable/disable LaTeX support
- `params.codeblocksdark` - dark theme for code blocks
- `menu.nav` - navigation menu

## Theme Documentation

Full documentation and examples are available in the `themes/hugo-tufte/exampleSite/` folder.
