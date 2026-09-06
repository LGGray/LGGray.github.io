# lggray.github.io

Single static page. No build step — edit `index.html`, commit, push.

## First-time deploy

1. On GitHub, create a **public** repo named exactly:

       LGGray.github.io

   (No README, no .gitignore — leave it empty.)

2. From this folder:

       git init
       git add .
       git commit -m "Initial site"
       git branch -M main
       git remote add origin https://github.com/LGGray/LGGray.github.io.git
       git push -u origin main

3. Repo → Settings → Pages → Source: "Deploy from a branch",
   branch `main`, folder `/ (root)`. Save.

4. Wait ~1 minute. Live at: https://lggray.github.io

## Updating

Edit `index.html`, then:

    git add -A && git commit -m "Update" && git push

Live site refreshes in under a minute.

## Placeholders still to fill

Search `index.html` for these:

- `YOUR-WORK-EMAIL` and `your.name@tum.de` — your work email
- `PUT-SCHOLAR-URL-HERE` — Google Scholar profile (delete the line if you don't have one)
- `PUT-BLUESKY-URL-HERE` / `@handle` — or delete that whole `<li>`

## Adding a paper

Copy one `<li>` block inside `<ul class="pubs">` and edit it.
Wrap your own name in `<span class="me">Gray LG</span>`.
Drop any link chip (DOI / PubMed / Code) you don't need.

## Custom domain (optional, ~€10/yr)

Buy a domain, add a file named `CNAME` containing just the bare domain
(e.g. `lachlangray.com`), then point a CNAME DNS record at `lggray.github.io`.
Re-enable "Enforce HTTPS" in Settings → Pages once it propagates.
