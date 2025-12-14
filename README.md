# Frappe Bible (from zero to hero)

A practical, example-driven guide to learning the Frappe Framework (v15). This repository contains the book content (Markdown), runnable example exercises, and CI to build and publish documentation using MkDocs + Material.

Goals
- Teach developers new to Frappe how to build apps, extend the framework, write server and client logic, test, and deploy.
- Provide runnable examples and lab exercises tied to chapters.

Quick start (local)
1. Clone this repo:
   git clone https://github.com/hamzabawumia/frappe-bible.git
2. Install dependencies for docs (optional):
   python -m pip install -r requirements.txt
3. Serve docs locally:
   mkdocs serve

Structure
- docs/           — chapters written in Markdown (MkDocs site)
- examples/       — runnable example apps and helper scripts
- exercises/      — lab exercises for hands-on learning
- .github/        — CI to build and publish docs to GitHub Pages

License
All files in this repository (book + examples) are released under the MIT License. See LICENSE.

Contributing
See CONTRIBUTING.md for guidelines on adding chapters, examples, and exercises.
