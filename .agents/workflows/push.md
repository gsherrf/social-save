---
description: Build, verify, and push the project to GitHub
---

# Push to GitHub

## Steps

1. Stage all changes
```bash
git add .
```

// turbo
2. Check the build for errors
```bash
npm run build
```

3. If the build fails, fix the errors and re-run step 2.

4. Commit the changes with a descriptive message
```bash
git commit -m "<descriptive message>"
```

// turbo
5. Push to GitHub
```bash
git push origin main
```

6. If the push fails (e.g. due to remote changes), pull first and retry:
```bash
git pull --rebase origin main
git push origin main
```
