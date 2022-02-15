# Hubbubooks

REST API to create, update and delete authors and books.

# Used technologies and languages:

node.js
express.js
mongoDB
filepond for design

javascript
html
css

# File structure

'public' folder - One file for filepond integration and all .css files for the project
'routes' folder - Routes for home, author and books pages
'views' folder - All remaining logic
  Here we have four folders:
    'authors' - all the files for form fields, new and edit functions, and show page for current author
    'books' - here files are the same as in the authors folder, but of course for books
    'layouts' - here we have one file, which include all css and js include scripts from filepond and main.css
    'partials' - One file for header which we use in every page. One for grid book information in book view stage. One for deleting form and one for error message where we have a validation. For example if you try to add a new author, but the field is empty, there you have an error message.
    In views folder we also have a index.ejs file for home page of the API
