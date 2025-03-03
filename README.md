# MkDocs Material Template

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit)
[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/bybatkhuu/docs.mkdocs-template/2.build-publish.yml?logo=GitHub)](https://github.com/bybatkhuu/docs.mkdocs-template/actions/workflows/2.build-publish.yml)
[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/bybatkhuu/docs.mkdocs-template?logo=GitHub&color=blue)](https://github.com/bybatkhuu/docs.mkdocs-template/releases)

This is a template repository for documentation projects using Material for MkDocs.

## ✨ Features

- **Material for MkDocs**: A Material Design theme for MkDocs.
- **Markdown Extensions**: Admonition, CodeHilite, Extra, Meta, Pymdown, Sane Lists, Toc, and more.
- **Customization**: Custom CSS, Favicon, Logo, Navigation, Search, and Social Links.
- **SEO Optimized**: Meta tags, Open Graph, Twitter Cards, and Google Analytics.
- **Responsive Design**: Mobile-friendly and optimized for small screens.
- **Syntax Highlighting**: Code blocks with line numbers and syntax highlighting.
- **Search Engine**: Full-text search with term highlighting.
- **Table of Contents**: Automatic table of contents for each page.
- **Navigation**: Sidebar navigation with collapsible sections.
- **Breadcrumbs**: Hierarchical navigation paths for each page.
- **Sitemap**: XML sitemap for search engines.
- **Blog Posts**: List of blog posts with tags and categories.
- **Mermaid Diagrams**: Flowcharts, sequence diagrams, Gantt charts, and more.
- **Math Equations**: LaTeX math equations with KaTeX support.
- **PlantUML Diagrams**: UML diagrams with PlantUML support.
- **FontAwesome Icons**: Scalable vector icons for buttons and links.
- **404 Page**: Custom 404 error page.
- **Redirects**: Custom 301 redirects for old URLs.
- **Dark Mode**: Toggle between light and dark themes.
- **Internationalization**: Multi-language support with translations.
- **Versioning**: Multiple versions of documentation with version selector.
- Project Structure
- Boilerplate/Template
- Best Practices
- Configuration
- Build
- Documentation
- Scripts
- CI/CD

## 🧩 Template

- You can use this template repository as reference to create a new repository with the same structure or clone the repository to start a new project. It will help you to organize your project structure and files. It works out of the box for most of the python projects.
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

---

## 🛠 Installation

### 1. 🚧 Prerequisites

- Install **Python (>= v3.9)** and **pip (>= 23)**:
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
pip install -r ./requirements.txt
```

### 4. 🏁 Serve documentation locally (for DEVELOPMENT or TEST)

```sh
./scripts/docs.sh
# Or:
mkdocs serve
```

### 5. 🏗️ Build documentation

Build the documentation into a static web (HTML) in the `site` directory:

```sh
./scripts/docs.sh -b
# Or:
mkdocs build
```

[TIP] Built static web can be published to any web server or cloud storage.

### 6. 🚀 Publish documentation (for PRODUCTION)

Build and push static web files into the `gh-pages` branch to deploy on GitHub Pages:

```sh
./scripts/docs.sh -p
# Or:
mkdocs gh-deploy --force
```

👍

---

## 📚 Documentation

- [Docs](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs)
- [Home](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/README.md)

### Getting Started

- [Prerequisites](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/getting-started/prerequisites.md)
- [Installation](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/getting-started/installation.md)

### Development

- [Docs](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/dev/docs.md)
- [Scripts](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/dev/scripts/README.md)
- [CI/CD](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/dev/cicd/README.md)
- [File Structure](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/dev/file-structure.md)
- [Sitemap](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/dev/sitemap.md)
- [Contributing](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/dev/contributing.md)
- [Roadmap](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/dev/roadmap.md)

### [Release Notes](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/release-notes.md)

### [Blog](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/blog/index.md)

### About

- [FAQ](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/about/faq.md)
- [Authors](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/about/authors.md)
- [Contact](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/about/contact.md)
- [License](https://github.com/bybatkhuu/docs.mkdocs-template/blob/main/docs/pages/about/license.md)

---

## 📑 References

- <https://squidfunk.github.io/mkdocs-material>
- <https://www.mkdocs.org>
- <https://mkdocstrings.github.io>
- <https://github.com/bharel/mkdocs-render-swagger-plugin>
