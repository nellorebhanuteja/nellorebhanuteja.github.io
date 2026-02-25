# Deploy to https://nellorebhanuteja.github.io/

Your site must be in the **nellorebhanuteja.github.io** repo to appear at the root URL.

## Steps

### 1. Create or use the user site repo

On GitHub, create (or use existing) repo: **nellorebhanuteja/nellorebhanuteja.github.io**

### 2. Push your code there

```bash
cd /mnt/c/Users/BhanuTejaNellore/Documents/my-cv-site

# Remove old remote if it points to my-cv-site
git remote remove origin 2>/dev/null || true

# Add the user site repo
git remote add origin https://github.com/nellorebhanuteja/nellorebhanuteja.github.io.git

# Push (force overwrites any existing content)
git push -u origin main --force
```

### 3. Configure GitHub Pages

- Repo → **Settings** → **Pages**
- **Source:** "Deploy from a branch"
- **Branch:** gh-pages | / (root)
- **Save**

### 4. Wait

The workflow will run, build Hugo, and push to `gh-pages`. Give it 1–2 minutes.

### 5. Open your site

https://nellorebhanuteja.github.io/

---

If the `nellorebhanuteja.github.io` repo already exists with other content, the `--force` push will replace it. Your Hugo site will take over.
