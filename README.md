# Git and GitHub Notes

A collection of useful Git and GitHub commands for everyday development.

## 🧑‍💻 Configure Git

```sh
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

## 🗂️ Initialize a Repository

```sh
git init
```

## 📌 Check File Status

```sh
git status
```

## ➕ Stage Files

- Add a specific file:
```sh
git add <filename>
```

- Add all files:
```sh
git add .
```

## ✅ Commit Changes

```sh
git commit -m "Your commit message"
```

## 📜 View Commit History

```sh
git log
```

## 🌿 Working with Branches

- Create a new branch:
```sh
git branch <branch-name>
```

- Create and switch to a branch:
```sh
git checkout -b <branch-name>
```

- Switch branches:
```sh
git checkout <branch-name>
```

- Return to main branch:
```sh
git checkout main
```

## 🌐 Remote Repository

- Add remote origin:
```sh
git remote add origin <repository-url>
```

- View remotes:
```sh
git remote -v
```

- Change remote URL:
```sh
git remote set-url origin <new-repository-url>
```

## 🚀 Push to GitHub

- First push (with upstream):
```sh
git push -u origin main
```

- Regular push:
```sh
git push origin main
```

- Push a new branch:
```sh
git push -u origin <branch-name>
```

## 🔄 Pull from GitHub

```sh
git pull origin main
```

## 🔐 Add SSH Key to GitHub

- Generate SSH key:
```sh
ssh-keygen -t ed25519 -C "your_email@example.com"
```

- Start ssh-agent and add the key:
```sh
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```

- Copy your public key:
```sh
cat ~/.ssh/id_ed25519.pub
```

- Add it to GitHub:
  - Go to **Settings > SSH and GPG keys > New SSH Key**
  - Paste your key


## 📥 Clone a Repository

Clone a remote repository to your local machine:

```sh
git clone <repository-url>
```

> Example:
```sh
git clone https://github.com/username/repo-name.git
```
