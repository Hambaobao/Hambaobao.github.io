# hambaobao.me

This is the source code for my personal website: [hambaobao.me](https://hambaobao.me/).  
The site is built with [Hugo](https://gohugo.io/) and automatically deployed to GitHub Pages using GitHub Actions.

## Features

- Powered by the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme
- Clean, fast, and fully static site
- Custom domain: `hambaobao.me`
- Automated deployment on every push to `main`

## Getting Started

### Prerequisites

- [Hugo](https://gohugo.io/getting-started/installing/) (extended version recommended)
- [Git](https://git-scm.com/)

### Installation

1. **Clone the repository:**
   ```sh
   git clone --recurse-submodules https://github.com/Hambaobao/hambaobao.github.io.git
   cd hambaobao.github.io
   ```

2. **Run the development server:**
   ```sh
   hugo server -D
   ```
   The site will be available at `http://localhost:1313/`.

### Configuration

- Main configuration: [`hugo.toml`](./hugo.toml)
- Theme: [PaperMod](https://github.com/adityatelange/hugo-PaperMod) (added as a submodule)
- Custom domain: [`CNAME`](./CNAME)

## Deployment

Deployment is handled automatically via GitHub Actions:

- On every push to the `main` branch, the workflow:
  1. Checks out the code (including submodules)
  2. Installs Hugo
  3. Builds the static site to the `public/` directory
  4. Publishes the contents of `public/` to the `gh-pages` branch using [peaceiris/actions-gh-pages](https://github.com/peaceiris/actions-gh-pages)

You can find the workflow configuration in [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml).

## License

This project is for personal use.  
Theme [PaperMod](https://github.com/adityatelange/hugo-PaperMod) is licensed under the MIT License. 