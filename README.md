# DevSecOps + AI Engineering Journey

**Building practical skills in Linux, Cloud Computing, Automation, DevSecOps, Security, and AI Engineering.**

Welcome to my engineering learning portfolio! This repository documents my journey toward becoming a DevSecOps and AI Engineer through structured learning, practical exercises, hands-on labs, technical documentation, and real-world projects.

My primary focus is to understand not only **how tools work**, but also **why they are used in production environments**.

**Primary Operating System:** Ubuntu Linux  
**Primary Cloud Platform:** Microsoft Azure  
**Version Control:** Git and GitHub  
**Learning Focus:** DevSecOps, Cloud Engineering, Automation, Security, and AI

---

## Learning Objectives

- Build strong Linux administration and troubleshooting skills.
- Master Git, GitHub, branching, and collaborative development workflows.
- Develop automation skills using Bash and Python.
- Learn containerization, CI/CD, infrastructure as code, and Kubernetes.
- Understand DevSecOps practices and secure software delivery.
- Gain hands-on experience with Microsoft Azure.
- Build AI-powered applications and integrate AI into engineering workflows.
- Maintain documented projects that demonstrate technical growth.

## Learning Methodology

Every learning module follows a practical approach:

1. **Understand** — Study concepts, commands, syntax, and underlying behavior.
2. **Practice** — Execute commands and complete exercises on Ubuntu.
3. **Troubleshoot** — Investigate errors and understand their causes.
4. **Document** — Record technical explanations and examples in `notes.txt`.
5. **Review** — Reinforce concepts using interview-style questions.
6. **Version Control** — Commit completed documentation and project code to GitHub.

---

# Completed Learning and Hands-on Practice

## Module 01 — Day 1: Linux Fundamentals

**Focus:** Linux command-line fundamentals, file management, permissions, basic administration, and Bash scripting.

### 1. Linux Fundamentals and Navigation

**Topics covered:**
- Introduction to Linux and the Ubuntu terminal
- Linux directory structure
- Current working directory
- Absolute and relative paths
- Home directory (`~`)
- Current directory (`.`) and parent directory (`..`)
- Hidden files and directories

**Commands practiced:**

| Command | Purpose |
|---|---|
| `pwd` | Display the current working directory |
| `ls` | List directory contents |
| `ls -la` | List files with detailed information, including hidden files |
| `cd` | Change the current directory |
| `cd ..` | Navigate to the parent directory |
| `cd ~` | Navigate to the home directory |

### 2. File and Directory Management

**Topics covered:**
- Creating files and directories
- Writing and reading file contents
- Standard output redirection
- Appending versus overwriting
- Copying files
- Moving and renaming files
- Deleting files and directories
- Editing files using Nano

**Commands practiced:**

| Command | Purpose |
|---|---|
| `mkdir` | Create a directory |
| `touch` | Create an empty file or update timestamps |
| `echo` | Print text |
| `>` | Redirect output and overwrite a file |
| `>>` | Append output to a file |
| `cat` | Display file contents |
| `cp` | Copy files |
| `mv` | Move or rename files |
| `rm` | Remove files |
| `nano` | Edit text files |

### 3. Linux File Permissions

**Topics covered:**
- Read (`r`), write (`w`), and execute (`x`) permissions
- Owner, group, and others
- Numeric permission representation
- Permissions such as `755`, `754`, `700`, and `644`
- Making scripts executable
- Basic permission-related security considerations

**Commands practiced:**

- `ls -l`
- `chmod 755`
- `chmod 644`
- `chmod 700`
- `chmod +x`

**Key learning:** Linux permissions control who can read, modify, or execute files and programs.

### 4. System Information and Resource Monitoring

**Topics covered:**
- Current user identification
- Hostname and kernel information
- System uptime
- Disk space usage
- Directory size
- Memory utilization

**Commands practiced:**

| Command | Purpose |
|---|---|
| `whoami` | Display the current username |
| `hostname` | Display the system hostname |
| `uname -r` | Display the Linux kernel version |
| `uptime` | Show system uptime and load averages |
| `df -h` | Display filesystem disk usage |
| `du -sh .` | Display the total size of the current directory |
| `free -h` | Display memory usage |

### 5. Linux Process Management

**Topics covered:**
- Running processes
- Process IDs (PIDs)
- Foreground and background processes
- Monitoring running processes
- Searching for specific processes
- Terminating processes
- Normal termination versus forced termination

**Commands practiced:**

- `ps`
- `ps aux`
- `ps -p`
- `top`
- `grep`
- `sleep 300 &`
- `kill`
- `kill -9`
- `Ctrl + C`

### 6. Package and Service Management

**Topics covered:**
- Administrator privileges and `sudo`
- APT package management
- Updating package indexes
- Installing and removing software
- Understanding Linux services
- Starting, stopping, restarting, and enabling services

**Commands practiced:**

- `sudo`
- `apt update`
- `apt upgrade`
- `apt install`
- `apt remove`
- `systemctl status`
- `systemctl start`
- `systemctl stop`
- `systemctl restart`
- `systemctl enable`
- `systemctl disable`

### 7. Bash Scripting Fundamentals

**Topics covered:**
- Introduction to Bash scripts
- The `#!/bin/bash` shebang
- Executing shell scripts
- Script permissions
- Combining Linux commands in a script

### Day 1 Project — Linux System Information Script

**File:** [`system-info.sh`](system-info.sh)

Created a Bash script that displays:

- Current user
- Hostname
- Linux kernel version
- System uptime
- Disk usage
- Memory usage

**Run the project:**

```bash
bash system-info.sh
```

**Learning outcome:** Developed foundational Linux administration skills and created a working system-information automation script.

---

## Module 02 — Git and GitHub Fundamentals

**Focus:** Version control, repository management, tracking changes, commits, and remote collaboration.

### Topics Covered

- Introduction to version control
- Difference between Git and GitHub
- Local and remote repositories
- Initializing a Git repository
- Understanding the `.git` directory
- Working Directory, Staging Area, and Commit History
- Tracked and untracked files
- Modified and staged file states
- Reviewing unstaged and staged changes
- Creating commits
- Writing meaningful commit messages
- Viewing commit history
- Understanding branches and commit IDs
- Connecting local repositories to GitHub
- Understanding `origin` and `main`
- Pushing commits to a remote repository

### Git Commands Learned

| Command | Purpose |
|---|---|
| `git init` | Initialize a Git repository |
| `git status` | Inspect repository state |
| `git diff` | Review unstaged changes |
| `git add <file>` | Stage selected changes |
| `git diff --staged` | Review staged changes |
| `git commit -m "message"` | Create a local commit |
| `git log --oneline` | View compact commit history |
| `git branch -M main` | Rename the current branch to `main` |
| `git remote add origin <url>` | Configure a remote repository |
| `git remote -v` | Display configured remote URLs |
| `git push` | Push commits to a remote |
| `git push -u origin main` | Push and configure upstream tracking |

### Hands-on Achievements

- Initialized a local Git repository on Ubuntu.
- Created a public GitHub repository.
- Connected the local repository to GitHub.
- Added technical notes and a Bash script to version control.
- Practiced reviewing, staging, and committing changes.
- Successfully pushed commits to GitHub.
- Practiced a repeatable Git documentation workflow.

**Learning outcome:** Built a foundation in Git-based version control and repository management.

---

## Module 03 — GitHub SSH Authentication

**Focus:** Secure GitHub authentication using SSH.

### Topics Covered

- SSH authentication fundamentals
- Public-key cryptography concepts
- Public and private SSH keys
- SSH key generation
- SSH agent basics
- SSH-based GitHub authentication
- SSH and HTTPS Git remote URLs
- Secure handling of credentials
- Protecting private keys and access tokens

### Commands Practiced

- `ssh-keygen`
- `ssh-agent`
- `ssh-add`
- `ssh -T git@github.com`
- `git remote -v`
- `git remote set-url`

### Hands-on Achievements

- Generated an SSH key pair on Ubuntu.
- Configured SSH authentication for GitHub.
- Verified successful GitHub SSH authentication.
- Changed the Git remote from HTTPS to SSH.
- Successfully pushed repository changes using SSH.

### Security Practices

- Private keys and authentication secrets remain outside the repository.
- No private SSH keys, passphrases, or personal access tokens are published.
- Documentation describes the authentication workflow without exposing sensitive credentials.

**Learning outcome:** Gained experience configuring secure, key-based GitHub access.

---

## Module 04 — Linux Administration and Log Analysis

**Focus:** Reading large files, monitoring logs, searching text, and combining Linux commands.

### Topics Covered

**File inspection**
- Displaying the first lines of a file
- Displaying the last lines of a file
- Reading large files interactively
- Monitoring continuously updated log files

**Log searching and filtering**
- Finding matching text
- Case-insensitive searches
- Displaying matching line numbers
- Excluding matching lines
- Counting matching lines

**Pipelines**
- Standard output and standard input
- Using pipes to connect commands
- Filtering process output

### Commands Practiced

| Command | Purpose |
|---|---|
| `head -n 20 notes.txt` | View the first 20 lines |
| `tail -n 30 notes.txt` | View the last 30 lines |
| `tail -f app.log` | Follow new log entries |
| `less notes.txt` | Read a large file interactively |
| `grep "ERROR" app.log` | Find matching log lines |
| `grep -i "error" app.log` | Search without case sensitivity |
| `grep -n "ERROR" app.log` | Display matching line numbers |
| `grep -v "INFO" app.log` | Exclude matching lines |
| `grep -c "ERROR" app.log` | Count matching lines |
| `ps aux \| grep bash` | Filter process information |

### Hands-on Practice

- Created a local application log file.
- Followed log updates in real time using `tail -f`.
- Practiced matching, excluding, and counting log entries.
- Used `less` to navigate longer files.
- Combined Linux commands using pipes.
- Practiced filtering running processes.

**Real DevOps relevance:** Log inspection and command-line filtering help troubleshoot applications, monitor systems, and investigate operational issues.

**Learning outcome:** Improved practical Linux troubleshooting and log-analysis skills.

---

## Module 05 — Git Collaboration, Branching, and Merging

**Focus:** Synchronizing repositories, isolated development, and integrating changes.

### 1. Git Pull and Git Fetch

**Topics covered:**
- Remote changes and local synchronization
- Differences between `git fetch` and `git pull`
- Reviewing remote commits before integration
- Comparing local and remote-tracking branches

**Commands practiced:**

- `git pull`
- `git pull --ff-only`
- `git fetch origin`
- `git log --oneline main..origin/main`
- `git diff main origin/main`

**Key learning:** `git fetch` downloads remote updates without automatically integrating them into the current branch, while `git pull` fetches and integrates changes.

### 2. Git Branch Management

**Topics covered:**
- Creating branches
- Listing branches
- Identifying the current branch
- Switching between branches
- Feature branch isolation
- Local and remote-tracking branches

**Commands practiced:**

- `git branch`
- `git branch -a`
- `git branch -r`
- `git branch --show-current`
- `git branch <name>`
- `git switch <name>`
- `git switch -c <name>`

### 3. Feature Branch Workflow

**Topics covered:**
- Creating feature branches
- Editing files on separate branches
- Staging and committing feature changes
- Maintaining independent branch histories
- Understanding when changes become part of `main`

### 4. Git Merge

**Topics covered:**
- Combining changes from different branches
- Understanding the current branch and incoming branch
- Fast-forward merges
- Merge commits
- Reviewing merge history

**Commands learned:**

- `git merge <branch>`
- `git merge --no-ff <branch>`
- `git merge --abort`
- `git log --oneline --graph --all`

**Learning outcome:** Practiced feature branch workflows and gained an understanding of collaborative Git development.

---

## Module 06 — Hands-on Git Merge Conflict Lab

**Focus:** Creating, investigating, resolving, and verifying a real Git merge conflict.

### Lab Objective

Simulate a configuration conflict between two development branches and resolve it safely.

**Environment:** Separate local Git practice repository on Ubuntu.

### Lab Scenario

Created a sample configuration file named `app.env`.

**Initial configuration:**

```env
APP_PORT=8000
```

Modified the same setting independently on two branches.

| Branch | Modified Setting |
|---|---|
| `main` | `APP_PORT=7000` |
| `feature-api` | `APP_PORT=9000` |

Both branches contained their own commits.

### Conflict Investigation

Attempted to merge `feature-api` into `main`.

Git identified conflicting changes in `app.env`.

Inspected the conflict using:

```bash
git status
cat app.env
```

The file contained Git conflict markers:

```text
<<<<<<< HEAD
APP_PORT=7000
=======
APP_PORT=9000
>>>>>>> feature-api
```

### Conflict Resolution

- Identified the current and incoming branch versions.
- Compared the conflicting configuration values.
- Selected `APP_PORT=9000` as the intended lab configuration.
- Removed the conflict markers using Nano.
- Staged the resolved file.
- Completed the merge.
- Verified the final configuration and commit history.

**Commands practiced:**

```bash
git merge feature-api
git status
nano app.env
git add app.env
git merge --continue
git log --oneline --graph --all
```

### Verified Commit History

The completed practice generated the following Git history:

```text
*   cdb0b9a (HEAD -> main) Merge branch 'feature-api'
|\
| * d7132a7 (feature-api) feat: change API port to 9000
* | c1c791f config: change main API port to 7000
|/
* 4a9ab65 chore: add initial app configuration
```

### Branch Cleanup

Practiced cleaning up a merged feature branch:

```bash
git branch -d feature-api
```

Learned the difference between safe branch deletion using `-d` and force deletion using `-D`.

### Lab Outcome

Successfully created and resolved a real Git merge conflict and examined the resulting merge commit graph.

**Note:** This was a local hands-on lab performed separately from the main GitHub repository. The lab results are documented here; the separate lab repository has not been published as part of this project.

---

# Project Portfolio

## Project 01 — Linux System Information Automation

**Technology:** Ubuntu Linux, Bash

**Repository file:** [`system-info.sh`](system-info.sh)

**Purpose:** Automate the collection of basic Linux system information.

**Key capabilities:**
- Current user information
- Hostname and kernel details
- System uptime
- Disk usage
- Memory usage

**Skills demonstrated:** Bash scripting, Linux administration, system inspection, and terminal automation.

## Lab 02 — Git Branching and Merge Conflict Resolution

**Technology:** Git, Ubuntu, Nano

**Purpose:** Practice collaborative development scenarios, including independent branches and conflicting configuration changes.

**Skills demonstrated:** Branch management, commits, merge conflict investigation, manual resolution, and commit history analysis.

**Availability:** Documented local lab, not a separate published repository.

---

# Repository Structure

Current primary project files:

```text
day-01-linux/
├── README.md
├── notes.txt
└── system-info.sh
```

| File | Description |
|---|---|
| `README.md` | Learning progress, technical topics, and hands-on project documentation |
| `notes.txt` | Detailed technical notes, command explanations, syntax, examples, and use cases |
| `system-info.sh` | Bash script for displaying Linux system information |

Additional local practice files, such as application logs and temporary configuration files, are kept separate from published project documentation.

---

# Learning Progress

| Learning Area | Progress |
|---|---|
| Ubuntu and Linux Fundamentals | Completed foundational exercises |
| File Management and Permissions | Practiced |
| Linux System Monitoring | Practiced |
| Package and Service Management | Practiced |
| Bash Scripting Fundamentals | Practiced |
| Linux System Information Script | Completed |
| Git and GitHub Fundamentals | Practiced |
| GitHub SSH Authentication | Configured and verified |
| Linux Log Analysis and Text Filtering | Practiced |
| Git Pull and Fetch | Studied and practiced |
| Git Branching and Switching | Practiced |
| Feature Branch Development | Practiced |
| Git Merge | Practiced |
| Merge Conflict Resolution Lab | Completed |
| Git Branch Cleanup | Practiced |
| Git Stash | Next hands-on topic |

*Progress labels distinguish foundational practice from advanced professional proficiency.*

---

# Upcoming Learning Roadmap

The following areas are planned for continued study and hands-on project development.

| Stage | Focus Areas |
|---|---|
| 1 | Advanced Linux Administration, Bash, Git, and Networking |
| 2 | Python Automation, FastAPI, and PostgreSQL |
| 3 | Docker and Containerization |
| 4 | GitHub Actions, CI/CD, and DevSecOps |
| 5 | Microsoft Azure and Terraform |
| 6 | Kubernetes, AKS, and Helm |
| 7 | GitOps, Security, and Observability |
| 8 | AI Engineering, LLMs, and RAG |
| 9 | AI Agents, Tool Calling, and AI Security |
| 10 | Final Secure Cloud-Native AI Platform |

These stages are learning goals, not claims of completed implementation.

---

# Engineering Practices

Throughout this journey, I aim to follow these principles:

- **Hands-on first:** Reinforce concepts by executing commands and building projects.
- **Understand the fundamentals:** Learn how tools behave instead of memorizing commands alone.
- **Document consistently:** Maintain technical explanations and reproducible learning notes.
- **Practice version control:** Review changes, write meaningful commits, and maintain repository history.
- **Build with security in mind:** Never commit private keys, credentials, access tokens, or application secrets.
- **Learn through troubleshooting:** Investigate failures and understand their root causes.
- **Improve incrementally:** Progress from foundational commands to integrated engineering projects.

---

# Long-Term Goal

My long-term goal is to develop the skills necessary to design, automate, secure, deploy, and monitor cloud-native applications.

The final portfolio objective is to build a **SecureAI Azure Platform** combining:

- Cloud infrastructure on Microsoft Azure
- Infrastructure as Code
- Containerized applications
- Automated CI/CD
- Kubernetes-based deployments
- Security scanning and DevSecOps controls
- Monitoring and observability
- AI/LLM integration and intelligent automation

This project is a future capstone goal and will be documented as development progresses.

---

# Repository Purpose

This repository serves as a continuously evolving technical learning portfolio.

It will include completed exercises, detailed notes, Bash and Python scripts, application projects, infrastructure automation, CI/CD workflows, security practices, and AI engineering projects as they are built.

**The objective is to demonstrate consistent learning, practical execution, technical understanding, and measurable progress toward DevSecOps and AI Engineering.**
