# Git Practical Assignment

This project demonstrates how to use Git and GitHub through practical tasks including branching, merging, and resolving conflicts.

## 👤 Author
**Name:** Aditya Anand Dande  
**Course:** AWS and DevOps – Fortune Cloud

---

## 📘 Step-by-Step Instructions

### 📝 Step 1: Create a New GitHub Repository
- Go to [GitHub](https://github.com/)
- Click **"New Repository"**
- Name it: `git-practice-task`
- Check **"Initialize with a README.md"**
- Click **"Create Repository"**

### 💻 Step 2: Clone Repository Locally
```bash
git clone <your-repo-url>
cd git-practice-task
```

### ✍️ Step 3: Modify `README.md` on `main`
- Open `README.md`
- Add your name and course info
```bash
git add README.md
git commit -m "Added name and course info"
git push origin main
```

### 🌿 Step 4: Create and Work on `feature-A` Branch
```bash
git checkout -b feature-A
```
- Create a new file named `index.html`
- Add sample HTML content:
```html
<!DOCTYPE html>
<html>
<head><title>Git Task</title></head>
<body><h1>Hello Git</h1></body>
</html>
```
```bash
git add index.html
git commit -m "Added index.html"
git push origin feature-A
```

### 🔀 Step 5: Create a Pull Request on GitHub
- Base: `main`
- Compare: `feature-A`
- Click **"Create Pull Request"**
- **Do not merge yet**

### 🌿 Step 6: Create Another Branch `feature-B`
```bash
git checkout -b feature-B main
```
- Modify the same lines in `index.html` for conflict
```bash
git add index.html
git commit -m "Conflicting change in index.html"
git push origin feature-B
```
- Create PR from `feature-B` to `main`

### ✅ Step 7: Merge `feature-A` First on GitHub

### ⚠️ Step 8: Merge `feature-B` (Conflict Expected)

### 🛠️ Step 9: Resolve Conflict Locally
```bash
git pull origin main
```
- Open `index.html`
- Resolve conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`)
```bash
git add index.html
git commit -m "Resolved conflict"
git push origin feature-B
```

### 🔚 Step 10: Complete the Merge on GitHub
---

## 🧠 Skills Practiced
- GitHub workflow
- Branching & merging
- Pull Requests & conflict resolution
- Writing markdown with images

