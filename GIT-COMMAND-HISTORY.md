# Git Command History

## Part 1
```bash
git init
git add .
git commit -m "Initial commit: setup project structure"
git branch -M main
git remote add origin <YOUR_GITHUB_REPOSITORY_URL>
git push -u origin main
```

## Part 2
```bash
git checkout -b feature-header
git add index.html
git commit -m "Add header component to index.html"
git push -u origin feature-header
git checkout main
git merge feature-header
git push origin main
```

## Part 3
```bash
git checkout -b nav-feature
git add index.html
git commit -m "Add primary navigation menu"
git checkout main
git checkout -b nav-alt
git add index.html
git commit -m "Add alternative navigation menu"
git checkout main
git merge nav-feature
git merge nav-alt
```

The second merge intentionally creates a conflict in `index.html`. The conflict markers are removed and both navigation menus are combined.

```bash
git add index.html
git commit -m "Resolve merge conflict between nav-feature and nav-alt"
git push origin main
```
