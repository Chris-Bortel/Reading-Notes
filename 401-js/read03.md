# Read: 03 - Data Modeling & NoSQL Databases
[README](/README.md)

## Reading Prompts
 Why would a developer choose to make data models? 
[Wikipedia Article](https://en.wikipedia.org/wiki/Data_model)
  - Data modeling allows the developer to sus out what the application is going to do, look like, and feel like. 
  - Allows developers to explore the flow of data and how each component relates to one another. 
  - Allows them to figure out what problems they are goiing to run into and figure out how to overcome them prior to starting a code base. 
  - This is also a way to have a discussion with the client in order to verify what they want and get an agreement that this is what the application will do.

What purpose do CRUD operations serve?
- Great article on [CRUD](https://www.codecademy.com/articles/what-is-crud)
- Create, Retrieve, Update, and Delete
- They are the four of the most basic functions of persistent storage
- It is what the web is built around. 

 What kind of database is Postgres? What kind of database is MongoDB?
- Postgres is a relational db
- MongoDB is schema-less, it  is documented based which uses collections to store the related information. 
- PostgreSQL is used mainly when static JSON is used and data is structured for SQL storage. 
- MongoDB is mainly used when data is unstructured and there is a need for modifying the JSON data inside the storage.


- What is Mongoose and why do we need it?
  - See below. 

- Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.





database
data model
CRUD -- 
  - Create -- HTTP POST method -- could be a function that would be called when something was being added to an application
  - Read -- HTTP GET -- could be a function whose purpose is to check whether an item is available
  - Update -- HTTP PUT -- function that allows the user to change values such as their name, address, birthday, etc.
  - DELETE -- HTTP DELETE -- function that allows the user to remove items/information from an app. 

schema [explained](https://www.youtube.com/watch?v=3BZz8R7mqu0)
- represents any kind of structure that us defined around the data. ( relationships, tables, fields, views, pachages, procedures, etc).
helps us understand what is going on inside of the database. It is the structure of the database. it is the folder that has the data  
sanitize

Structured Query Language (SQL)
Non SQL (NoSQL)

MongoDB 
-  documented based which uses collections to store the related information.
- Does not use tables and columns, instead it uses documents and collections... 
- used for writing the dynamic queries as it is designed for working the continuously changing data. It also provides good performance and provides the functionality of automatic sharding(a method for distributing data across multiple machines.).

Mongoose explained briefly...[Stackchief: Top 4 reasons to use mongoose with mongoDB](https://www.stackchief.com/blog/Top%204%20Reasons%20to%20Use%20Mongoose%20with%20MongoDB)
  - Mongoose is an object document modeling (ODM) layer that sits on top of Node's MongoDB driver. (It helps in organizing the data stored in the db)
  -  it saves time writing your own validations and instance methods
  
record
document
Object Relation Mapping (ORM)