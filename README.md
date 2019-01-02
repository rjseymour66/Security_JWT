# Here are the commands to get going:
npm i express
npm i mongoose
npm i nodemon
npm i body-parser

npm i --save-dev babel-cli babel-preset-env babel-preset-stage-0

** create .babelrc in root and add the following ** 

{
  "presets": [
    "env",
    "stage-0"
  ]
}

** add this to the scripts in package.json **

"start": "nodemon ./index.js --exec babel-node -e js"

* create the following folders:
	src
	src > controllers
	src > models
	src > routes

## Manually Secure Node project
1. Start mongo in the terminal
2. npm install --save jsonwebtoken bcrypt
3. create new controllers/models

## Make first Postman call
1. localhost:3000/auth/register
2. Header: x-www-form-urlencoded
3. Enter params:
  - userName:
  - email:
  - password:

4. change path to localhost:3000/auth/login
5. change to localhost:3000/contact
  - In Headers, add Authorization parameter and 'JWT jalskdjfls;jdkfajskdlfjasdjf' (key info)
