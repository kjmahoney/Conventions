#MEAN Convention

##Setting up MONGOOSE

###Setting up the db

`Npm init -y`
`npm install --save mongoose (npm i -S mongoose)``
`mkDir db`
####Connection.js
`Require mongoose`
`Mongoose.connect`
`mongoose.connect("mongodb://localhost/[name]")`

Export the module
Touch models.js
Require connection.js
Create schema
Export

Module.exports = {
 		Url: mongoose.model(“Url”,UrlSchema),
	}

Touch seeds.js
Require connection and model
Define seed data (either in file or sepearate json)
Declare model
Drop database and seed
Test is out
show dbs - Show a list of all databases
use database-name - Connect to a database
show collections - List the collections in a database
db.students.find() - List all students in a student collection

EXPRESS


Npm init -y (if not ran before)

Npm i -S Express, hbs, body-parser
touch index.js
Require express
Var express = require(“express”)
Create a variable to invoke it
var app = express();
App.listen
Require other stuff!
 mongoose
Any models you’ll be using
Set and Uses
Set your port
Set your view engine
Set your routes
GET or POST
MkDir Views
Layout.hbs
{{{body}}} (can use engine to customize)
Set styles
MkDir public
app.use(“/assets”, express.static(“public”)
