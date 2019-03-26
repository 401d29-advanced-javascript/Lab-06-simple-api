##Lab-6-simpe-api

##Author
--Aaron Bruce

##Links Resouces
--github link:
--travis link:

##Documentation
--jsdocs:
--swagger
##Modules
--

##Setup
--npm init
--npm install http eslint

##Running the app
--In terminal
~$ json-server --watch= ./db.json

--To add an object (POST)
In another terminal
--to create a category object
~$ echo '{"name":"Some Name", "display_name":"Some Display Name", "description":"Some Description"} | http POST :3000/categories/

--To make a product object
~$ echo '{"name":"Some Name", "display_name":"Some Display Name", "description":"Some Description"} | http POST :3000/products/

--To DELETE a category object
~$ http DELETE :3000/categories/id
EX: http DELETE :3000/categories/1

--To DELETE a product object
~$ http DELETE :3000/products/#id

--To PUT (update) an object
~$ echo '{"name":"Aaron"} | http PUT :3000/categories/id
EX: echo '{"name":"Aaron"} | http PUT :3000/categories/1

To READ all objects
~$ http READ :3000/categories
OR
~$ http READ :3000/products

--To READ one object
~$ http READ :3000/products/id