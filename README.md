# MARV Platform & Getting Started Documentation

This repository contains the official **MARV** (*Managed Activities, Review, and Validation*) documentation series built with **Sphinx** and formatted in **reStructuredText (`.rst`)** using the **Read The Docs** theme.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Documentation Structure](#documentation-structure)
- [Prerequisites](#prerequisites)
- [Setup & Installation](#setup--installation)
- [Building the Documentation](#building-the-documentation)
- [Previewing Locally](#previewing-locally)
- [Deploying to Read The Docs](#deploying-to-read-the-docs)

---

## 📖 Overview

MARV is an integrated platform designed for building and experiencing interactive developer education natively within Visual Studio Code. This documentation portal covers:

1. **Platform Overview:** Purpose, architecture, and core workflow of MARV.
2. **Installation Guide:** Installing the extension manually from VSIX package (`.vsix`).
3. **API Endpoint Configuration:** Connecting to the institution API server (`https://marv.computing.edgehill.ac.uk`).
4. **Student ID Setup:** Configuring student identification for course progress tracking.
5. **Interface Navigation:** Understanding modules (☁️ Cloud vs 🔒 Lock), tutorials, and pages.
6. **Workspace Management:** Setting up working directories in VS Code.
7. **Reference & Troubleshooting:** Configuration cheat sheet and troubleshooting guide.

---

## 📂 Documentation Structure

```text
.
├── docs/
│   ├── .readthedocs.yaml         # Read The Docs v2 build configuration
│   ├── requirements.txt          # Python build dependencies
│   ├── Makefile                  # Build automation for Unix/macOS
│   └── source/
│       ├── conf.py               # Sphinx configuration & RTD theme settings
│       ├── index.rst             # Main documentation entry point & TOC
│       ├── _static/
│       │   ├── custom.css        # Custom callouts & styling
│       │   └── images/           # Screenshots and animated GIFs
│       ├── getting_started/      # Getting started tutorials series
│       │   ├── index.rst
│       │   ├── 01_about.rst
│       │   ├── 02_installation.rst
│       │   ├── 03_api_setup.rst
│       │   ├── 04_student_id.rst
│       │   ├── 05_interface.rst
│       │   └── 06_workspaces.rst
│       └── reference/            # Directive reference & troubleshooting
│           ├── index.rst
│           ├── cheat_sheet.rst
│           └── troubleshooting.rst
└── README.md                     # This build and deployment guide
```

---

## ⚙️ Prerequisites

Before building the documentation, ensure your environment has:

- **Python:** Version 3.8 or higher.
- **Pip:** Python package manager.
- **Virtual Environment Tool:** `venv` module (included with Python 3).

---

## 🚀 Setup & Installation

Follow these steps to prepare your build environment:

### 1. Navigate to Project Directory
```bash
cd "Marv Tutotial Assets"
```

### 2. Create and Activate Virtual Environment

**macOS / Linux:**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

**Windows (PowerShell):**
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Install Required Dependencies
```bash
pip install -r docs/requirements.txt
```

---

## 🛠️ Building the Documentation

### Standard Build Command (Sphinx CLI)
To build HTML documentation, run:

```bash
sphinx-build -E -W --keep-going -b html docs/source docs/build/html
```

### Clean Rebuild via Makefile
```bash
make -C docs clean html
```

---

## 🌐 Previewing Locally

Preview the compiled documentation site locally in your web browser:

```bash
python3 -m http.server 8000 --directory docs/build/html
```
Open your browser and navigate to `http://localhost:8000`.

---

## ☁️ Deploying to Read The Docs

1. Commit your changes and push your repository to **GitHub** or **GitLab**.
2. Sign in to your account on [Read The Docs](https://readthedocs.org).
3. Click **Import a Project** and select your repository.
4. Read The Docs will automatically detect `docs/.readthedocs.yaml` and publish your hosted site.
