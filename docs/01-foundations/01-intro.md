# Part I — Foundations

## Chapter 1 — Introduction to Frappe (v15)

Objectives
- Understand what Frappe is and when to use it
- Learn core concepts: Sites, Apps, Bench, Workers, Redis, MariaDB
- Create a minimal local site and app (guided)

What is Frappe?
Frappe is a full-stack, batteries-included web framework written in Python and JavaScript. It offers an integrated ORM, UI framework, REST API, background workers, and a set of tools (bench) to manage sites and apps.

Core concepts (short)
- bench: developer tool to manage Frappe sites and apps
- site: an isolated instance that contains the database and files for an installation
- app: a package that contains DocTypes, pages, hooks, and business logic
- DocType: Frappe's schema + controller for a model (table)

Try it — create a local site and app (Frappe v15)
Prerequisites: Python 3.11+, Node.js 18+, Yarn, Redis, MariaDB. For development you can use the official bench or Docker.

Commands (classic bench method)

1. Install bench CLI (global):
   python -m pip install --upgrade frappe-bench

2. Create a bench folder and init (this may download Frappe/ERPNext code or you can use Docker):
   bench init frappe-bench --frappe-branch version-15
   cd frappe-bench

3. Create a new site:
   bench new-site site1.local

4. Create a new app:
   bench new-app first_app

5. Install the app on your site:
   bench --site site1.local install-app first_app

6. Start the development server:
   bench start

After the server starts, open http://localhost:8000 and log in (admin user created during new-site).

Note: Commands and branches may change; consult official Frappe docs for the latest platform-specific install notes.

Summary
This chapter introduced core Frappe concepts and gave quick commands to create a local site and app for v15.
