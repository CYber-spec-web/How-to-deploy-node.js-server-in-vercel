# How-to-deploy-node.js-server-on-vercel

# 1. prepare file 🗃️🗃️


### before deployment, you have to do something.  


#### . You should have the node.js file
if you don't know how to make the node.js file. go to here

![image](https://github.com/CYber-spec-web/How-to-deploy-node.js-server-on-vercel/blob/main/that%20is%20a%20image%20folder%2C%20ignore%20it/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202021-08-16%20183018.png)

#### . You should have a node.js server file
like this
````
var express = require('express');
var app = express();

app.get('/', function (req, res) {
   res.send('Hello World');
})

var server = app.listen(process.env.PORT || 3000, function () {
   console.log("server start running");
})
````
if you don't know how to make a node.js server file. go to here

#### . In the ```` package.json ````
variable "main" must be ```` index.js ```` (important)  
while your server file name must be ```` index.js ```` also (important)
// for my experience, vercel could only read index.js


#### . For library install
you may install the library that you want with command
````
npm install --save <library name>
````
so that the library file will save in ```` /node_modules ```` and library data will save in ```` package.json ````  
To let vercel server can read library successfully  


#### . You should have a ```` vercel.json ```` file.
you have to put vercel.json in the main directory
````
Folder
|
|_vercel.json
````
the ````vercel.json```` file was be put on the file area  
you can download it and save it in the main directory


# 2. make a github project


### The easy way to deploy app on vercel is to put the project in github and connect to vercel.  
### So first, we have to make a github project.  
