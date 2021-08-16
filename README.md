# How-to-deploy-node.js-server-on-vercel

# 1. prepare file

. You should have a node.js folder

. In the package.json 
variable "main" must be index.js (important)
while your server file name must be index.js also(important)
// for my experience, vercel could only read index.js

. For library install
you may install the library that you want with command
````
npm install --save <library name>
````
then, your library folder will save in ```` /node_modules ```` by auto
