# Savvy Tech website

Portfolio website for Savvy Tech, featuring website and graphic design projects.

## Files

```
index.html     The website (single page)
logo/          Savvy Tech logo files (transparent SVG and PNG)
.nojekyll      Tells GitHub Pages to serve the files as they are
README.md      This file
```

## Publish on GitHub Pages (no software needed)

1. Sign in at github.com. Click the **+** at the top right, then **New repository**.
2. Name it. Two options:
   - `yourusername.github.io` gives you the address `https://yourusername.github.io`
   - Any other name, such as `savvy-tech`, gives you `https://yourusername.github.io/savvy-tech`
3. Set it to **Public**, leave everything else unticked, and click **Create repository**.
4. On the next screen, click **uploading an existing file**.
5. Unzip `savvy-tech.zip` on your computer. Open the unzipped folder, select everything inside it (index.html, the logo folder, README.md, .nojekyll) and drag it all into the upload box. Do not upload the zip file itself, GitHub will not unzip it.
6. Scroll down and click **Commit changes**.
7. Go to **Settings**, then **Pages** in the left menu. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main** and folder to **/ (root)**. Click **Save**.
8. Wait one to two minutes and refresh the Pages screen. Your live address appears at the top with a **Visit site** button.

Note: `.nojekyll` starts with a dot, so Windows and Mac may hide it. The site still works without it, so don't worry if it doesn't upload.

## Updating the site

Open the repository, click **Add file**, then **Upload files**, and drop in the changed files. Files with the same name are replaced. Click **Commit changes** and the live site updates within a minute or two.

## Using your own domain (optional)

1. In **Settings > Pages**, type your domain (for example `savvytech.gd`) under **Custom domain** and click **Save**.
2. At your domain registrar, add these DNS records:
   - Four **A** records for `@` pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153` and `185.199.111.153`
   - One **CNAME** record for `www` pointing to `yourusername.github.io`
3. Once the domain connects (can take up to 24 hours), tick **Enforce HTTPS** on the Pages screen.

## Using Git from the command line (optional)

```
cd savvy-tech
git init
git add .
git commit -m "Savvy Tech website"
git branch -M main
git remote add origin https://github.com/yourusername/savvy-tech.git
git push -u origin main
```

Then turn on Pages as in step 7 above.
