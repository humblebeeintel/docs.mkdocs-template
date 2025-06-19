# MkDocs Material Template

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit)
[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/bybatkhuu/docs.mkdocs-template/2.create-release.yml?logo=GitHub)](https://github.com/bybatkhuu/docs.mkdocs-template/actions/workflows/2.create-release.yml)
[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/bybatkhuu/docs.mkdocs-template?logo=GitHub&color=blue)](https://github.com/bybatkhuu/docs.mkdocs-template/releases)

This is a template repository for documentation, wiki, knowledge base and technical blog using **Material for MkDocs**.

## ✨ Features

- MkDocs Material
- Wiki/Knowledge base
- Technical blog
- Markdown support
- Static site generator
- Project Structure
- Boilerplate/Template
- Best Practices
- Configuration
- Documentation
- Scripts
- CI/CD

## 🧩 Template

- You can use this template repository as reference to create a new repository with the same structure or clone the repository to start a new project. It will help you to organize your project structure and files. It works out of the box for most of the documentation projects.
- You can customize (remove, modify or add) the files and directories as needed to meet your project requirements.
- If you want to use the template repository directly, just click the **[Use this template](https://github.com/new?template_name=docs.mkdocs-template&template_owner=bybatkhuu)** button and follow the instructions.
- You can use **cookiecutter** to generate a new project from **[cookiecutter](https://github.com/bybatkhuu/docs.mkdocs-template/tree/cookiecutter)** branch:

    ```sh
    # Clone the cookiecutter branch:
    git clone -b cookiecutter https://github.com/bybatkhuu/docs.mkdocs-template.git

    # Install cookiecutter:
    pip install cookiecutter

    # Generate a new project from the cookiecutter template:
    cookiecutter -f ./docs.mkdocs-template
    ```

---

## 🛠 Installation

### 1. 🚧 Prerequisites

- Install **Python (>= v3.10)** and **pip (>= 23)**:
    - **[RECOMMENDED] [Miniconda (v3)](https://www.anaconda.com/docs/getting-started/miniconda/install)**
    - *[arm64/aarch64] [Miniforge (v3)](https://github.com/conda-forge/miniforge)*
    - *[Python virutal environment] [venv](https://docs.python.org/3/library/venv.html)*

[OPTIONAL] For **DEVELOPMENT** environment:

- Install [**git**](https://git-scm.com/downloads)
- Setup an [**SSH key**](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh) ([video tutorial](https://www.youtube.com/watch?v=snCP3c7wXw0))

### 2. 📥 Download or clone the repository

**2.1.** Prepare projects directory (if not exists):

```sh
# Create projects directory:
mkdir -pv ~/workspaces/projects

# Enter into projects directory:
cd ~/workspaces/projects
```

**2.2.** Follow one of the below options **[A]**, **[B]** or **[C]**:

**OPTION A.** Clone the repository:

```sh
git clone https://github.com/bybatkhuu/docs.mkdocs-template.git && \
    cd docs.mkdocs-template
```

**OPTION B.** Clone the repository (for **DEVELOPMENT**: git + ssh key):

```sh
git clone git@github.com:bybatkhuu/docs.mkdocs-template.git && \
    cd docs.mkdocs-template
```

**OPTION C.** Download source code:

1. Download archived **zip** file from [**releases**](https://github.com/bybatkhuu/docs.mkdocs-template/releases).
2. Extract it into the projects directory.

### 3. 📦 Install dependencies

```sh
# Install 'mkdocs-material' and other dependencies:
pip install -r ./requirements.txt
```

### 4. 🏁 Run the documentation server locally (for DEVELOPMENT)

```sh
mkdocs serve -a 0.0.0.0:8000
# Or:
./scripts/docs.sh
```

### 5. 🌐 Check the documentation in web browser

- <http://localhost:8000>

### 6. 🏗️ Generate the HTML documentation files (static site)

```sh
mkdocs build
# Or:
./scripts/docs.sh -b

# Check the generated HTML files (it should be in the `site` directory):
ls -al ./site
```

### 7. 🚀 Deploy the documentation

```sh
# Copy the generated HTML files to the web server:
cp -r ./site/* /var/www/docs.example.com/public
# Or deploy the documentation to GitHub Pages (branch: gh-pages) of the current repository:
mkdocs gh-deploy
```

👍

---

## 📑 References

- <https://squidfunk.github.io/mkdocs-material>
- <https://squidfunk.github.io/mkdocs-material/getting-started>
- <https://www.mkdocs.org>
- <https://pypi.org/project/mkdocs-material>
- <https://mkdocstrings.github.io>
- <https://github.com/bharel/mkdocs-render-swagger-plugin>
- <https://github.com/blueswen/mkdocs-swagger-ui-tag>
