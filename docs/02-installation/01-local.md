# Installation — Local (short)

This chapter outlines a minimal local development setup using the official bench CLI. It is intentionally brief; for production and platform-specific notes see later chapters.

Prerequisites
- Python 3.11+
- Node.js 18+
- Yarn
- Redis
- MariaDB (10.6+ recommended)

Quick steps (repeat of intro with a few notes)

1. Install bench CLI: python -m pip install --upgrade frappe-bench
2. Initialize bench: bench init frappe-bench --frappe-branch version-15
3. Create a site: bench new-site site1.local
4. Create and install app: bench new-app first_app && bench --site site1.local install-app first_app
5. Start bench: bench start

Docker option: Later chapters will include a full docker-compose example used in CI for examples.
