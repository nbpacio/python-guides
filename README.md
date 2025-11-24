# Python Programming Guide

This guide provides a list of instructions for setting up a Python programming environment.

## Getting Started

Follow these steps to create a local development environment.

### 1. Create a Local Repository Folder

```powershell
mkdir your_project_name
cd your_project_name
```

### 2. Create and Activate a Virtual Environment

Creating a virtual environment ensures that project dependencies are isolated.

```powershell
python -m venv .venv
```

To activate the virtual environment, use the appropriate command for your operating system.

**Windows (PowerShell):**
```powershell
.venv\Scripts\Activate.ps1
```

**Linux/macOS (Bash):**
```bash
source .venv/bin/activate
```

### 3. Create a `.gitignore` File

A `.gitignore` file specifies intentionally untracked files that Git should ignore. It's crucial to create this *before* initializing a Git repository to prevent sensitive files or unnecessary directories from being committed.

Create a `.gitignore` file and add the following content:

```
# Virtual environments
.venv
venv/
env/
ENV/

# Environment variables
.env
*.env
```

### 4. Initialize Git

Initialize a Git repository in your project folder (make sure you are not inside the `.venv` directory).

```powershell
git init
```

### 5. Create Project Files

You can create files using the command line.

**Windows (PowerShell):**
```powershell
echo "# Your project's main script" > main.py
```
*Note: Use `>>` to append content to a file instead of overwriting it.*

**Linux/macOS (Bash):**
```bash
touch main.py
```

### 6. Install Python Modules

Install necessary Python packages into your activated virtual environment.

```powershell
pip install python-dotenv openai
```

### 7. Create a `requirements.txt` File

A `requirements.txt` file lists all the Python dependencies for your project. This allows other developers to easily install the required packages.

Create a `requirements.txt` file with the following content:

```
python-dotenv>=1.0.0
openai>=1.0.0
```
