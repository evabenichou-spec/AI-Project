# Publish your Meeting Notebook (GitHub Pages)

Your notebook is **`meeting-notebook.html`**. The repo root also has **`index.html`**, which redirects to it so your site URL can be short.

## One-time: turn on GitHub Pages

1. Push this repo to GitHub (see below).
2. On GitHub: **Settings → Pages** (under “Code and automation”).
3. Under **Build and deployment**:
   - **Source**: Deploy from a branch.
   - **Branch**: `main` (or `master`), folder **`/ (root)`**.
4. Save. After ~1 minute, your site will be at:

   **`https://evabenichou-spec.github.io/AI-Project/`**

   That URL loads `index.html`, which sends you to `meeting-notebook.html`.

## Push from your Mac (if not already published)

```bash
cd "/Users/eva.benichou/My notebook/Notebook/Learning Cursor"
git add meeting-notebook.html index.html NOTEBOOK-PUBLISH.md
git commit -m "Add Meeting Notebook and GitHub Pages entry"
git push origin main
```

If `git push` asks for login, use a [Personal Access Token](https://github.com/settings/tokens) as the password, or switch the remote to SSH.

## Data stays in your browser

Notes and files are stored in **IndexedDB** on each device/browser. The hosted URL is only the app; it does not upload your notes to GitHub.

## Other hosts (optional)

You can also upload **`meeting-notebook.html`** (and **`index.html`** if you want a root URL) to **Netlify Drop**, **Cloudflare Pages**, or any static host.
