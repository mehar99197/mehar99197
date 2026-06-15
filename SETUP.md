# 🚀 How to publish your GitHub Profile README

Your GitHub **profile** README is a special repository that must be named **exactly the same as your username**: `mehar99197`.
When that repo has a `README.md` at its root, GitHub shows it at the top of your profile page.

---

## ✅ Option A — Web (easiest, no terminal)

1. Go to **https://github.com/new**
2. **Repository name:** `mehar99197`  ← must match your username exactly
3. Set it to **Public** and tick **“Add a README file”**
4. Click **Create repository**
5. Open the repo → edit `README.md` → paste the contents of this folder's `README.md` → **Commit changes**
6. Upload the images: in the repo click **Add file → Upload files**, drop the `assets/` folder (avatar.png, profile-transparent.png, profile-trimmed.png), commit.
7. (Optional snake animation) **Add file → Create new file**, name it `.github/workflows/snake.yml`, paste this folder's `snake.yml`, commit. Then go to the **Actions** tab and run **“Generate Contribution Snake”** once.

---

## ✅ Option B — Git CLI (from this folder)

```bash
cd github-profile

git init -b main
git add .
git commit -m "✨ Professional profile README"

# create the repo on GitHub (needs GitHub CLI `gh` authenticated)
gh repo create mehar99197 --public --source=. --remote=origin --push

# ...or if you created the empty repo manually on github.com:
# git remote add origin https://github.com/mehar99197/mehar99197.git
# git push -u origin main
```

> 🔑 If `gh` isn't logged in, run `gh auth login` first (or in this chat type:
> `! gh auth login` to run it interactively).

---

## 🖼️ Using your background-removed photo

`assets/` contains three ready-to-use versions of your photo:

| File | Use it for |
| ---- | ---------- |
| `avatar.png` | **GitHub profile picture** (circular, head-and-shoulders) — Settings → Profile → upload |
| `profile-transparent.png` | Full cut-out with transparent background — slides, portfolio, banners |
| `profile-trimmed.png` | Transparent cut-out cropped tight to your body |

To set your profile picture: **github.com → Settings → Profile → Profile picture → Edit → Upload a photo** → choose `avatar.png`.

---

## 🔧 Personalize before publishing

In `README.md`, replace the placeholder `#` links in the **Connect** section with your real:
- LinkedIn URL
- HackerOne / Bugcrowd profile
- LeetCode / Codeforces handle

Everything else (stats, streak, trophies, languages) auto-fills from your `mehar99197` activity once the repo is live.
