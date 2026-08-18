# How to Contribute

Follow these steps exactly — this is the same process used for real open
source projects on GitHub.

## 1. Fork the repository

Click the **Fork** button at the top-right of this repo's GitHub page.
This creates a copy of the repo under your own GitHub account.

## 2. Clone your fork

On your computer, open a terminal and run (replace `your-username`):

```bash
git clone https://github.com/your-username/REPO_NAME.git
cd REPO_NAME
```

## 3. Add the original repo as "upstream" (optional but recommended)

```bash
git remote add upstream https://github.com/ORIGINAL_OWNER/REPO_NAME.git
```

This lets you pull in future updates from the original repo later.

## 4. Create a new branch

Never work directly on `main`. Create a branch named after what you're doing:

```bash
git checkout -b add-your-name
```

## 5. Make your change

Open `contributors.md` in any text editor and add one line at the bottom
of the list, in this format:

```markdown
- [Your Name](https://github.com/your-username)
```

Save the file.

## 6. Commit your change

```bash
git add contributors.md
git commit -m "Add [Your Name] to contributors list"
```

## 7. Push your branch to your fork

```bash
git push origin add-your-name
```

## 8. Open a Pull Request

1. Go to your fork on GitHub.
2. You'll see a banner: **"add-your-name had recent pushes"** with a
   **Compare & pull request** button — click it.
3. Add a short title and description of your change.
4. Click **Create Pull Request**.

## 9. Wait for review

The repo maintainer will review your PR and merge it. Once merged, check
`contributors.md` on the main repo — your name will be there permanently!

---

### Common issues

- **"Permission denied" when pushing** → You're pushing to the original repo
  instead of your fork. Check your `origin` remote with `git remote -v`.
- **Merge conflicts** → Someone else added their name near yours. Pull the
  latest `main` from `upstream`, rebase your branch, and resolve the
  conflict in `contributors.md`.
- **Forgot to branch** → If you committed on `main` in your fork, that's
  okay — you can still open a PR from `main`, but branching is best
  practice for future contributions.
