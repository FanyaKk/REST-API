# Hubbubooks

REST API to create, update and delete authors and books.

# Features

- Add Authors
- Add Books
- Search by different criteria
- Edit and delete functions for both ( books and authors )

# Used technologies and languages:

node.js
express.js
mongoDB
filepond for design

javascript
html
css

# File structure and description

- 'public' folder - One file for filepond integration and all .css files for the project
- 'routes' folder - Routes for home, author and books pages
- 'views' folder - All remaining logic
  Here we have four folders:
    - 'authors' - all the files for form fields, new and edit functions, and show page for current author
    - 'books' - here files are the same as in the authors folder, but of course for books
    - 'layouts' - here we have one file, which include all css and js include scripts from filepond and main.css
    - 'partials' - One file for header which we use in every page. One for grid book information in book view stage. One for deleting form and one for error message where we have a validation. For example if you try to add a new author, but the field is empty, there you have an error message.
    In views folder we also have a index.ejs file for home page of the API.
- In the .env file is database url connection to mongo db and in server.js is the rest of logic for connecting to db and express.

# Mongo DB account for testing

To connect to the database you can use this link:

mongodb+srv://<username>:<password>@mongodbcluster.7feon.mongodb.net/myFirstDatabase?retryWrites=true&w=majority
and replace <username> and <password> with following

username: test-user
password: 7DtHYhKVnkth7Pot

# Installation
 
This is a [Node.js](https://nodejs.org/en/) module available through the
[npm registry](https://www.npmjs.com/). Installation is done using the
[`npm install` command](https://docs.npmjs.com/getting-started/installing-npm-packages-locally)

Run
To start local server you need to use `npm run devStart` command and open https://localhost:3000
In the `package.json` file we have a dependencies which allow us automatically refresh our server everytime we make a change  

"devDependencies": {
    "dotenv": "^16.0.0",
    "nodemon": "^2.0.15"
  }
