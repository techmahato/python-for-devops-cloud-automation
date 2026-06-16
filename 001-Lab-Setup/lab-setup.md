# Python Lab Setup on Windows Laptop

## Complete Python Bootcamp For DevOps & Cloud — From Zero to Hero 2026

This guide walks you through setting up your complete Python development environment on a Windows laptop for DevOps and Cloud Automation.

---

## Table of Contents

1. [Introduction to Python for DevOps](#1-introduction-to-python-for-devops)
2. [Python Lab Setup on Laptop](#2-python-lab-setup-on-laptop)
3. [VS Code IDE vs Kiro IDE](#3-vs-code-ide-vs-kiro-ide)

---

## 1. Introduction to Python for DevOps

### 1.1 What is a Programming Language?

A programming language is a set of instructions that tells a computer what to do. Just like humans communicate using English, Hindi, etc., we communicate with computers using programming languages like Python, Java, Go, etc.

**Examples:** Python, JavaScript, Go, Java, C++

### 1.2 What is the Meaning of Scripting Using Python for DevOps?

In DevOps, **scripting** means writing small programs (scripts) to **automate repetitive tasks** such as:

- Deploying applications to servers
- Managing cloud infrastructure (AWS, Azure, GCP)
- Monitoring system health
- Automating CI/CD pipelines
- Parsing log files
- Managing configurations

Python is the most popular scripting language in DevOps because it is simple, readable, and has powerful libraries for automation.

### 1.3 Python for Developers vs Python for DevOps

| Aspect | Python for Developers | Python for DevOps |
|--------|----------------------|-------------------|
| Focus | Building applications (web apps, APIs, software) | Automating infrastructure & operations |
| Libraries | Django, Flask, FastAPI | Boto3, Paramiko, Ansible, Terraform SDK |
| Output | Web apps, APIs, desktop apps | Scripts, automation tools, pipelines |
| Goal | Create products for end users | Automate, monitor, and manage systems |
| Example | Build a REST API | Write a script to auto-scale EC2 instances |

### 1.4 Why Should You Learn Python in 2026 as a DevOps / SRE / Platform Engineer?

1. **Most in-demand scripting language** — Almost every DevOps job description mentions Python
2. **Cloud automation** — AWS (Boto3), Azure (Azure SDK), GCP all have Python SDKs
3. **Infrastructure as Code** — Tools like Ansible use Python internally
4. **CI/CD pipelines** — Automate Jenkins, GitHub Actions, GitLab CI with Python
5. **Monitoring & Alerting** — Build custom monitoring scripts
6. **Kubernetes & Containers** — Python clients for K8s API
7. **Easy to learn** — Clean syntax, beginner-friendly, huge community
8. **Career growth** — Moves you from manual operations to automation-first engineering

---

## 2. Python Lab Setup on Laptop

### 2.1 Understand Python Interpreter and IDE (VS Code)

| Component | What It Is | Why You Need It |
|-----------|-----------|-----------------|
| **Python Interpreter** | The engine that reads and executes your Python code | Without it, your computer can't run `.py` files |
| **VS Code (IDE)** | A code editor where you write, edit, and debug code | Makes coding easier with features like auto-complete, syntax highlighting, and extensions |

**Think of it this way:**
- Python Interpreter = The engine of a car (makes it run)
- VS Code IDE = The dashboard and steering wheel (makes it easy to drive)

---

### 2.2 Install Python on Your Windows Laptop

#### Step 1: Download Python

1. Open your browser
2. Go to: [https://www.python.org/downloads/](https://www.python.org/downloads/)
3. Click **"Download Python 3.x.x"** (latest version)

#### Step 2: Install Python

1. **Double-click** the downloaded `.exe` file
2. ⚠️ **IMPORTANT:** Check the box ✅ **"Add python.exe to PATH"** (at the bottom of installer)
3. Click **"Install Now"**
4. Wait for installation to complete
5. Click **"Close"**

#### Step 3: Verify Installation

Open **Command Prompt** (search "cmd" in Start menu) and type:

```cmd
python --version
```

**Expected Output:**
```
Python 3.x.x
```

Also verify pip (Python's package manager):

```cmd
pip --version
```

**Expected Output:**
```
pip 24.x.x from ... (python 3.x)
```

> ✅ If you see version numbers, Python is installed successfully!

---

### 2.3 Install VS Code IDE on Your Windows Laptop

#### Step 1: Download VS Code

1. Go to: [https://code.visualstudio.com/download](https://code.visualstudio.com/download)
2. Click **"Windows"** download button

#### Step 2: Install VS Code

1. Double-click the downloaded `.exe` file
2. Accept the agreement
3. ✅ Check **"Add to PATH"**
4. ✅ Check **"Register Code as an editor for supported file types"**
5. ✅ Check **"Add 'Open with Code' action to Windows Explorer file context menu"**
6. ✅ Check **"Add 'Open with Code' action to Windows Explorer directory context menu"**
7. Click **Install** → Click **Finish**

#### Step 3: Verify Installation

Open Command Prompt and type:

```cmd
code --version
```

You should see the VS Code version number.

---

### 2.4 Optimize Your VS Code IDE for DevOps & Automation

#### 2.4.1 Create Project Folder

1. Create a folder on your system for all Python DevOps projects:

```
D:\python-for-devops-cloud-automation\
```

2. Open VS Code
3. Go to **File → Open Folder** → Select your project folder
4. OR use the shortcut: **Shift + Right-Click** on the folder → **"Open with Code"**

#### 2.4.2 Enable Auto Save

Auto Save ensures you never lose your work.

1. Open VS Code
2. Go to **File → Auto Save** (click to enable ✅)
3. OR go to **File → Preferences → Settings** → Search "Auto Save" → Set to `afterDelay`

Now your files will be saved automatically!

#### 2.4.3 Install VS Code Extensions for DevOps Productivity

Extensions add powerful features to VS Code. Here are the must-have extensions:

| # | Extension Name | What It Does |
|---|---------------|--------------|
| 1 | **Python** (by Microsoft) | Python code support — IntelliSense, linting, debugging, formatting, and code structure |
| 2 | **Prettier - Code Formatter** | Automatically formats your code to look clean and consistent |
| 3 | **Better Comments** | Improves code commenting with color-coded annotations (alerts, TODOs, informational notes) |
| 4 | **Live Server** | Launches a local development server with live reload for static & dynamic pages |
| 5 | **AWS Toolkit** | Connect to AWS services, manage Lambda, CloudWatch, S3 directly from VS Code |

#### How to Install Extensions:

1. Open VS Code
2. Click the **Extensions icon** on the left sidebar (or press `Ctrl + Shift + X`)
3. Search for the extension name
4. Click **Install**

##### Extension 1: Python (by Microsoft)

```
Search: "Python"
Publisher: Microsoft
```

**What it gives you:**
- Syntax highlighting for `.py` files
- IntelliSense (auto-complete suggestions)
- Code linting (error detection)
- Debugging support
- Code formatting

##### Extension 2: Prettier - Code Formatter

```
Search: "Prettier - Code formatter"
Publisher: Prettier
```

**What it gives you:**
- Auto-formats your code on save
- Consistent code style across your project

##### Extension 3: Better Comments

```
Search: "Better Comments"
Publisher: Aaron Bond
```

**What it gives you:**
- Color-coded comments:
  - `// !` → Red (alerts/warnings)
  - `// ?` → Blue (questions)
  - `// TODO` → Orange (todos)
  - `// *` → Green (highlights)

##### Extension 4: Live Server

```
Search: "Live Server"
Publisher: Ritwick Dey
```

**What it gives you:**
- One-click local server for HTML/CSS/JS files
- Auto-refresh browser when you save changes

##### Extension 5: AWS Toolkit

```
Search: "AWS Toolkit"
Publisher: Amazon Web Services
```

**What it gives you:**
- Manage AWS resources from VS Code
- Deploy Lambda functions
- View CloudWatch logs
- S3 bucket management

---

### 2.5 Install and Configure Kiro CLI Agent in VS Code Terminal

Kiro CLI is an AI-powered coding agent that helps you create Python projects, explain complex code, and boost productivity directly from your terminal.

#### Step 1: Install Kiro CLI

1. Open VS Code Terminal (`Ctrl + ~`)
2. Follow the official Kiro CLI installation guide for Windows
3. Verify installation:

```cmd
kiro --version
```

#### Step 2: Configure Kiro CLI

1. Authenticate Kiro CLI with your account
2. Set up your workspace preferences
3. Start using Kiro in your terminal to:
   - Generate Python code
   - Explain complex functions
   - Create project structures
   - Debug errors

#### What Kiro CLI Helps You With:

- 🚀 **Create Python projects** — Scaffold project structure instantly
- 🧠 **Explain complex code** — Ask Kiro to break down any function or module
- 🐛 **Debug errors** — Paste error messages and get solutions
- 📝 **Write documentation** — Generate docs for your code

---

## 3. VS Code IDE vs Kiro IDE

### 3.1 What is Kiro?

Kiro is an **AI-powered development environment** built by Amazon. It combines the traditional code editor experience with intelligent AI assistance that helps you write, understand, and ship code faster.

### 3.2 What is Kiro IDE?

Kiro IDE is a **full GUI-based development environment** (like VS Code) that comes with built-in AI capabilities. It's designed to be your AI pair programmer that understands your codebase and helps at every step.

### 3.3 Kiro IDE vs VS Code IDE

| Feature | VS Code | Kiro IDE |
|---------|---------|----------|
| **Type** | Code Editor + Extensions | AI-native IDE |
| **AI Integration** | Requires extensions (Copilot, etc.) | Built-in AI agent |
| **Spec-driven development** | Not available | Built-in (Requirements → Design → Tasks) |
| **Hooks & Automation** | Manual configuration | Built-in event-driven hooks |
| **Steering (Project Rules)** | Not available | Built-in via `.kiro/steering/` |
| **MCP Support** | Limited | Native MCP server support |
| **Price** | Free | Free (with AI features) |
| **Best For** | General development | DevOps automation with AI assistance |

### 3.4 Install Kiro IDE (GUI) on Windows Laptop

#### Step 1: Download Kiro

1. Go to: [https://kiro.dev](https://kiro.dev)
2. Click **Download for Windows**
3. Download the `.exe` installer

#### Step 2: Install Kiro

1. Double-click the downloaded installer
2. Follow the installation wizard
3. Launch Kiro after installation
4. Sign in with your account

#### Step 3: Verify

- Open Kiro IDE
- Create a new file → It should work like VS Code with AI features built-in

### 3.5 Install Kiro CLI on Windows Laptop

Kiro CLI gives you Kiro's AI capabilities directly in your terminal (works inside VS Code terminal too).

#### Installation:

1. Open Command Prompt or PowerShell
2. Follow the installation instructions from [https://kiro.dev/cli](https://kiro.dev/cli)
3. Verify:

```cmd
kiro --version
```

### 3.6 Kiro IDE for DevOps - Why It's Useful

| Use Case | How Kiro Helps |
|----------|---------------|
| Writing automation scripts | AI generates Python scripts for AWS, Docker, K8s |
| Understanding legacy code | Ask Kiro to explain any function or module |
| Building CI/CD pipelines | Kiro helps write pipeline configs |
| Debugging infrastructure issues | Paste errors, get solutions |
| Spec-driven development | Plan features with Requirements → Design → Tasks |
| Code reviews | AI reviews your code for best practices |

### 3.7 Install Extensions in Kiro IDE for DevOps

Install the **Python** extension in Kiro IDE:

1. Open Kiro IDE
2. Go to Extensions (`Ctrl + Shift + X`)
3. Search and install: **Python** (by Microsoft)

> Kiro IDE already has AI built-in, so you need fewer extensions compared to VS Code.

---

## 4. Lab Setup Checklist ✅

Use this checklist to confirm everything is set up correctly:

| # | Task | Status |
|---|------|--------|
| 1 | Python installed and `python --version` works | ⬜ |
| 2 | pip installed and `pip --version` works | ⬜ |
| 3 | VS Code installed and `code --version` works | ⬜ |
| 4 | Python extension installed in VS Code | ⬜ |
| 5 | Prettier extension installed | ⬜ |
| 6 | Better Comments extension installed | ⬜ |
| 7 | Live Server extension installed | ⬜ |
| 8 | AWS Toolkit extension installed | ⬜ |
| 9 | Auto Save enabled in VS Code | ⬜ |
| 10 | Project folder created and opened in VS Code | ⬜ |
| 11 | Kiro CLI installed and working | ⬜ |
| 12 | Kiro IDE installed (optional) | ⬜ |
| 13 | Python extension installed in Kiro IDE | ⬜ |

---

## 5. Quick Verification - Run Your First Python File

After setup, verify everything works end-to-end:

### Step 1: Create a test file

In your project folder, create a file named `test_setup.py`:

```python
# Lab Setup Verification Script
print("✅ Python is working!")
print("✅ VS Code is configured!")
print("✅ Lab setup is complete!")
print(f"Python version check passed!")
```

### Step 2: Run it

Open terminal in VS Code (`Ctrl + ~`) and type:

```cmd
python test_setup.py
```

### Expected Output:

```
✅ Python is working!
✅ VS Code is configured!
✅ Lab setup is complete!
Python version check passed!
```

> 🎉 If you see this output, your lab is ready! You can now start learning Python for DevOps & Cloud Automation.

---

## What's Next?

Now that your lab is set up, we move to:
- **002: Mini Python Projects** — Start writing real Python code
- Learn Python syntax, variables, data types, and more!

---

> **Tip:** Bookmark this page. If you ever reinstall your system or set up a new machine, come back here and follow these steps again.
