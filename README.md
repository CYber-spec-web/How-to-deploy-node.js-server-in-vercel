# How-to-deploy-node.js-server-on-vercel

# 1. prepare file 🗃️🗃️


. You should have the node.js file
if you don't know how to make the node.js file. go to here


. You should have a node.js server file
if you don't know how to make a node.js server file. go to here


. In the ```` package.json ````
variable "main" must be ```` index.js ```` (important)  
while your server file name must be ```` index.js ```` also (important)
// for my experience, vercel could only read index.js


. For library install
you may install the library that you want with command
````
npm install --save <library name>
````
so that the library file will save in ```` /node_modules ```` and library data will save in ```` package.json ````  
To let vercel server can read library successfully  


. You should have a ```` vercel.json ```` file.
