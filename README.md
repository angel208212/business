# Jalapeños — website files for GitHub Pages

This folder is the whole website: one page, its photo, its styles, and a small
script that fades sections in as you scroll.

## 1. Put it on GitHub Pages

1. Go to github.com and create a **new repository** (name it anything, e.g. `jalapenos`).
2. On the repository page click **Add file → Upload files**, then drag everything in
   this folder in (`index.html`, `app.js`, `assets`, `README.md`, `.nojekyll`).
3. Click **Commit changes**.
4. Go to **Settings → Pages**.
5. Under **Build and deployment → Source**, choose **Deploy from a branch**.
6. Branch: `main` (or `master`), folder: `/ (root)`, then **Save**.
7. Wait about a minute. Your address appears there, like
   `https://YOUR-USERNAME.github.io/jalapenos/`.

## 2. Add your own domain

Buy a domain first (Namecheap, Cloudflare, GoDaddy, or a `.bz` registrar all work).
Two names that were still free when this page was built:
`jalapenosbelize.com` and `jalapenossanignacio.com`.

Then, at the company where you bought the domain, add these DNS records:

| Type  | Name / Host | Value                        |
| ----- | ----------- | ---------------------------- |
| A     | @           | 185.199.108.153              |
| A     | @           | 185.199.109.153              |
| A     | @           | 185.199.110.153              |
| A     | @           | 185.199.111.153              |
| CNAME | www         | YOUR-USERNAME.github.io      |

Next, in the repository: **Settings → Pages → Custom domain**, type your domain
(e.g. `jalapenosbelize.com`), click **Save**, and tick **Enforce HTTPS** once the
domain shows as connected.

GitHub writes a `CNAME` file into the repository for you. If you would rather add
it by hand, create a file named `CNAME` in this folder containing only your domain
on the first line, e.g. `jalapenosbelize.com`.

DNS can take anywhere from a few minutes to a day to switch over.

## 3. Editing the page

Open `index.html` in any text editor. The dish list, the guest quotes, the opening
hours and the address are all plain text in that one file — change the words, save,
and upload the file again to GitHub to publish the change.
