# 📂 Dotfiles Manager

A simple and modular **dotfiles management system** that helps you:

* 🔄 **Backup** your dotfiles into a repo
* ☁️ **Sync** dotfiles across machines or VMs
* ⚡ **Install** dotfiles on a new system quickly without manual setup

This repo contains my personal dotfiles by default, but you can replace them with your own and use the scripts to manage your environment.

---

## 🚀 Features

* **Backup script** → saves selected dotfiles into the repo
* **Sync script** → pulls the latest dotfiles and updates them locally
* **Install script** → sets up a new system with your dotfiles in one command
* **Customizable** → easily swap my dotfiles with your own
* **Safe** → excludes sensitive files (SSH keys, API keys, GPG keys, etc.)

---

## 📂 Repository Structure

```
dotfiles-manager/
│
├── dotfiles/               # Your backed-up dotfiles (replace mine with yours)
│   ├── .bashrc
│   ├── .vimrc
│   ├── .zshrc
│   └── ...
│
├── scripts/                # Core management scripts
│   ├── backup.sh           # Backup selected dotfiles into dotfiles/
│   ├── sync.sh             # Sync repo dotfiles → local system
│   ├── install.sh          # Install dotfiles on a new machine
│   └── utils.sh            # Shared helper functions (optional)
│
├── .gitignore              # Ignore sensitive/unwanted files
├── LICENSE                 # License (MIT or your choice)
└── README.md               # Project documentation
```

---

## ⚡ Usage

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/dotfiles-manager.git
cd dotfiles-manager
```

### 2. Backup your dotfiles

```bash
./scripts/backup.sh
```

This copies selected dotfiles from your home directory into the `dotfiles/` folder.

### 3. Sync dotfiles

```bash
./scripts/sync.sh
```

This updates your local dotfiles from the repo (or vice versa).

### 4. Install dotfiles

```bash
./scripts/install.sh
```

This copies dotfiles from the repo into your home directory. Perfect for fresh installs or new VMs.

---

## ⚠️ Disclaimer

* The dotfiles included here are **my personal setup**.
* If you want to use this project, **replace the contents of the `dotfiles/` folder with your own files**.
* **Never commit sensitive files** (SSH keys, API keys, GPG private keys, etc.). Add them to `.gitignore`.

---

## 🔧 Future Improvements (optional ideas)

* Add **interactive menu** to select which dotfiles to install/backup
* Add **symlink management** (using GNU `stow` or `ln -s`) instead of direct copy
* Add **package installer script** for dependencies (e.g., zsh, vim plugins, tmux)
* Add **OS detection** (Ubuntu, Arch, Fedora) for cross-distro setup

---
