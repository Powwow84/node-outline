## How to set up Node/NPM project

1. Make a directory in the terminal using mkdir
2. npm init -y ..... initializes NPM
3. touch index.js ....  js file can be named anything, this is the entry point
4. npm i express .... tells express npm to install express
5. echo "node_modules" >> .gitignore .... creates an ignore file and adds node_modules to it. this will make it so when we add to git it doesnt add the modules to the respository
6. const express = require('express') .... this part is required to run express. the variable express can be named anything but must require('express)
7. const app = express() .... initializes express
8. Create a home route example:

app.get('/', (req, res) => {
    res.send('Hello, World!');
});

app.listen(8000);
