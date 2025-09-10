# GitHub Pages Starter

A minimal, fast, accessible static site you can deploy via GitHub Pages and connect to a custom domain.

## Quick start

1. Create a new repo named `<username>.github.io` (or any name for a project page).
2. Upload these files to the repo root and commit.
3. In **Settings → Pages**, choose the branch (`main`) and root folder (`/`). Save.
4. (Optional) In **Settings → Pages**, set your **Custom domain** and save. This creates/updates the `CNAME` file.
5. Configure your DNS at your registrar (see below), then wait for DNS to propagate. Enable **Enforce HTTPS** when available.

## DNS for custom domain

- **Apex domain** (`example.com`): create four `A` records pointing to GitHub Pages:
  - 185.199.108.153
  - 185.199.109.153
  - 185.199.110.153
  - 185.199.111.153
- **www subdomain** (`www.example.com`): create a `CNAME` to `<username>.github.io`

You can also point other subdomains (like `blog.example.com`) via CNAME to `<username>.github.io`.

## Notes
- Update the placeholder text in `index.html` with your info.
- Add more pages by creating additional `.html` files and linking to them.
- Want a 404 page? Create `404.html` in the root.
