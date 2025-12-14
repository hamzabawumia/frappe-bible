# First App — Tutorial

Objectives
- Scaffold a minimal app
- Create a simple DocType and form
- Add a server-side method and a client script

Scaffold (commands)

1. From your bench folder:
   bench new-app library
   bench --site site1.local install-app library

2. Create a DocType (via UI or JSON). Example fields: Title (Data), Author (Data), Published Date (Date).

3. Add a server method in library/library/doctype/book/book.py:

   def on_insert(self):
       # example: set a default value or call an external service
       pass

4. Add a client script to validate or enhance UX (assets/js/book.js).

Try it: Add 3 book records and build a simple report.

Challenge: Add a scheduled job that emails a weekly digest of recent books.
