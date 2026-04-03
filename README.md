# Computational Reasoning and Discovery Lab

This repository contains the website for the **Computational Reasoning and Discovery Lab**.
The site is designed to be easily editable by lab members. Most content is written in Markdown, making it simple to add or update pages without needing extensive web development experience.

---

# Overview

The website is built with:

- **Jekyll** (static site generator)
- **Ruby** (required runtime)
- **Bundler** (dependency manager)

Content editing mostly involves modifying **Markdown (.md) files**, while styling is handled using **HTML and CSS**.

---

# Initial Setup (First Time Only)

Follow these steps to run the website locally.

## 1. Install Ruby

Download and install Ruby from:

```
https://rubyinstaller.org/
```

During installation:

1. Choose the **recommended Ruby version**
2. At the final stage, **run `ridk install` when prompted**

When the `ridk` window opens, select:

```
3 - MSYS2 and MINGW development toolchain
```

This installs required native extensions needed for Jekyll.

---

## 2. Install Jekyll and Bundler

Open a **new terminal** (Command Prompt, PowerShell, or Git Bash) and run:

```
gem install jekyll bundler
```

This installs the tools used to build and serve the website.

---

## 3. Clone the Repository

Clone the website repository to your machine.

Example:

```
git clone <repository-url>
cd <repository-folder>
```

---

## 4. Install Project Dependencies

Inside the repository folder run:

```
bundle install
```

This installs all dependencies defined in the project's `Gemfile`.

---

## 5. Run the Website Locally

Start the local development server with:

```
bundle exec jekyll serve
```

Once running, open your browser and go to:

```
http://localhost:4000
```

The website will automatically rebuild whenever you modify files.

---

# Editing the Website

Most of the website is written using **Markdown files (.md)**.

General rule:

- **Content → Markdown**
- **Layout / styling → HTML & CSS**

This means most edits can be done without touching the site's styling.

---

# Adding Lab Members

To add a new person to the website:

## Step 1 — Add the Photo

Place the person's image inside:

```
assets/img/people
```

Use a clear filename, for example:

```
assets/img/name_last.jpeg
```

---

## Step 2 — Create a Markdown File

Inside the folder:

```
_people/
```

Create a new `.md` file:

```
jane_doe.md
```

---

## Step 3 — Fill in the Person Details

Each person file contains structured metadata (front matter).  
Fill in the appropriate fields such as name, role, email, and photo.

After saving, the person will automatically appear on the **People** page.

---

# Adding Projects

Projects follow a similar structure.

## Step 1 — Add Project Images

Place images inside:

```
assets/img/
```

---

## Step 2 — Add a Project File

Inside:

```
_projects/
```

create a new Markdown file:

```
reasoning_project.md
```

---

## Step 3 — Fill in Project Metadata

### Important: Quadrant Tags

Each project **must include a tag indicating its quadrant**.

These tags are used by the website to place projects in the correct section.

Make sure the correct quadrant tag is included.

---

# Adding Teaching Content or Courses

Teaching pages follow essentially the **same process as projects**.

---

# Editing Existing Pages

To modify existing pages:

1. Locate the corresponding Markdown file.
2. Edit the content using standard Markdown syntax.
3. Save the file.

The site will **automatically rebuild locally** if `jekyll serve` is running.

---

# Styling Changes

If you need to modify the **appearance** of the website:

- Layout files are located in:

```
_layouts/
```

- Styling is located in:

```
_assets/css/
```

These files use **HTML, Liquid templates, and CSS**.

Only modify these if you need to change the structure or visual style of the website.

---

# Maintainers

Computational Reasoning and Discovery Lab  
Website maintained by lab members.
