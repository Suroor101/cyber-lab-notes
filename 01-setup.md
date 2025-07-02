### `01-setup.md`

# 01 - Tool Installation and Git Basics

This document outlines the full setup process for a cybersecurity lab, including virtualization tools, Kali Linux, development environment setup, and version control using Git and GitHub.

---

## 1. VMware Workstation Player

**Download Link:**  
https://www.vmware.com/products/workstation-player.html

**Installation Steps:**
1. Sign in to Broadcom
1. Downloaded the installer for the host OS.
2. Ran installer and accepted default installation options.
3. Launched VMware .

---

## 2. Kali Linux Virtual Machine

**Download Link:**  
https://www.kali.org/get-kali/

**Setup Procedure:**
1. Downloaded the Kali Linux `.ova` image from the official site.
2. Imported the `.ova` into VMware via `File → Open`.
3. Configured VM settings (NAT networking, sufficient RAM/storage).
4. Started the VM, logged in using default credentials (`kali:kali`).
5. Updated the OS:
   ```bash
   sudo apt update && sudo apt upgrade -y
   ````

---

## 3. Visual Studio Code (VS Code)

**Download Link:**
[https://code.visualstudio.com/](https://code.visualstudio.com/)

**Installation Steps:**

1. Download the Installer File.
5. Install VScode:
   ```bash
   sudo apt install ./<file_name>
   ````
3. Launched VS Code to verify installation.
4. Install useful extensions


---

## 4. Git


**Download Link:**
[https://git-scm.com/downloads](https://git-scm.com/downloads)

**Installation Steps:**

1. Downloaded and installed Git.
2. Verified installation:

   ```bash
   git --version
   ```
3. Configured global user settings:

   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"
   ```

---

## 5. Local Git Repository Initialization

You created the local Git repository with the following commands:

```bash
mkdir cyber-lab-notes
cd cyber-lab-notes
git init
```

* `git init` initialized the `.git` directory, making this a local repository.
* Created files like `01-setup.md` (this file), and staged/committed them.

```bash
git add 01-setup.md
git commit -m "Add initial setup notes"
```

---

## 6. GitHub Repository Setup and Push

Created a GitHub repository named `cyber-lab-notes` (without README initialization). You then connected and pushed your local repo:

```bash
git remote add origin https://github.com/<username>/cyber-lab-notes.git
git branch -M main
git push -u origin main
```

After that to run:

```bash
git add 01-setup.md
git commit -m "Tool installation and Git setup documentation"
git push
````


* `origin` was set to the remote GitHub URL.
* `main` was created/renamed as the default branch and pushed.

---

## 7. Git Basics Practiced

You used the following Git commands:

* `git init` – Create a new local repository.
* `git add` – Stage changes for commit.
* `git commit -m "..."` – Record changes in repository.
* `git push` – Send commits to GitHub (`main` branch).
* `git clone` – Copy the repository to another location or machine:


---