JWT Tokens Auth

https://scotch.io/tutorials/authenticate-a-node-es6-api-with-json-web-tokens


packages
npm install express body-parser bcrypt dotenv jsonwebtoken mongoose  --save
npm install morgan nodemon cross-env  --save-dev

Why these dependencies?
Dependencies

    body-parser:  This will add all the information we pass to the API to the request.body object.
    bcrypt:       We'll use this to hash our passwords before we save them our database.
    dotenv:       We'll use this to load all the environment variables we keep secret in our .env file.
    jsonwebtoken: This will be used to sign and verify JSON web tokens.
    mongoose:     We'll use this to interface with our mongo database.

Development dependencies

    morgan:       This will log all the requests we make to the console whilst in our development environment.
    nodemon:      We'll use this to restart our server automatically whenever we make changes to our files.  cross-env:    This will make all our bash commands compatible with machines running windows. 

Express package.json add to scripts:
    "dev": "cross-env NODE_ENV=development nodemon index.js"
Run Server: npm run dev
