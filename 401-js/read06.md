# Read: 06 - HTTP and REST

[README](/README.md)

Why would a developer choose to make data models? [bridging the gap](https://www.bridging-the-gap.com/3-reasons-to-data-model/)
- To understand the flow and the relationship of data with in an application, and how each aspect of the application works with each other. 
- we can delete fields that we do not want prior to building the db
- you can change attributes and anything else


What purpose do CRUD operations serve? [Create, read, update and delete](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete)
- It lets us keep the applications dynamic. The entire internet is based on this principle
  - Create: adds data from the user 
  - Read: retrieves the data
  - Update: edit or update existing data
  - Delete: remove data


What kind of database is Postgres? What kind of database is MongoDB?
- Postgres is a relational db which mean that it has tables, rows, and columns. It is a sql( structured query language) type db 
- PostgreSQL is used mainly when static JSON is used and data is structured for SQL storage. 
- MongoDB is mainly used when data is unstructured and there is a need for modifying the JSON data inside the storage.
- MongoDB is schema-less, or a NoSQL db, it  is documented based which uses collections to store the related information. 


What is Mongoose and why do we need it?
[Stackchief: Top 4 reasons to use mongoose with mongoDB](https://www.stackchief.com/blog/Top%204%20Reasons%20to%20Use%20Mongoose%20with%20MongoDB)
  - Mongoose is an object document modeling (ODM) layer that sits on top of Node's MongoDB driver. (It helps in organizing the data stored in the db)
  -  it saves time writing your own validations and instance methods


Describe how NoSQL Databases scale horizontally [Scaling Horizontally and vertically for DBs](https://medium.com/@abhinavkorpal/scaling-horizontally-and-vertically-for-databases-a2aef778610c)
- means that they are scaled by adding more machines in the pood of resources insted of adding more power
- we do this by adding replicas and sectioning off the code data from eachother...?


Give one strong argument for and against NoSQL Databases
- It is difficult to change a large chunk of data 
- you cannot use joins which add flexibilty to a data model. If order to make it work without joins, you have to design the db very carefully so that you do not have to build an entirely new data structure to handle the new data. 


Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.

Name 3 cloud based NoSQL Databases
- AWS
- MongoDB
- Google cloud platform



## Term Definitions
<!-- database
data model -->
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
- is a language that is used for accessing and minipulating databases. This is a relational db
Non SQL (NoSQL)
- does not use relational storage. good for storing data of differing data types

MongoDB 
-  documented based which uses collections to store the related information.
- Does not use tables and columns, instead it uses documents and collections... 
- used for writing the dynamic queries as it is designed for working the continuously changing data. It also provides good performance and provides the functionality of automatic sharding(a method for distributing data across multiple machines.).

Mongoose explained briefly...[Stackchief: Top 4 reasons to use mongoose with mongoDB](https://www.stackchief.com/blog/Top%204%20Reasons%20to%20Use%20Mongoose%20with%20MongoDB)
  - Mongoose is an object document modeling (ODM) layer that sits on top of Node's MongoDB driver. (It helps in organizing the data stored in the db)
  -  it saves time writing your own validations and instance methods
  
record
- is the way that data entries are stored in a SQL db
document. They use rows and columns to organize data. 
- is the way that entries are stored in a NoSQL db
Object Relation Mapping (ORM)
- a way of converting data from one incompatible system type to another. Wikipedia says that it essentially, "Create a virual object db that can be used within the programming language. 

Preview Preparation Materials 
- [Youtube Explanation of a RESTful API, REST, and HTTP](https://www.youtube.com/watch?v=Q-BpqyOT3a8&t=28s)

1. Which 3 things had you heard about previously and now have better clarity on?
- api : I did not realize that an api was a contract between two pieces of software
- rest: Representational State Transfer, lets us use http to transfer the data that the server is grabbing
  - relies on a statekless, clent-server protocol

  HTTP Methods(just a reminder): GET, POST, PUT, DELETE
  - there are also less used methods:
    - HEAD: sam as get, but does not return a body. 
    - OPTIONS: Returns a list of the supported http methods
    - PATCH: update partial resources

  - I did not realize that adding 1 to user user/1 will look up only one user vs just user which grabs all of them.
  - github has an API!

  OAUTH: We can use the token within a parameter

  - I had not even thought about the user within the request. ``GET /user/:username`` --- the colon denotes a place holder

  - within the response, I di not realize that it had information about how many repositories it has
  2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - REST
  - Stateless Servers?
  - Tell me more about how the internet works.


  3. What are you most excited about trying to implement or see how it works?
  - I want to learn about OAUTH
  - I am super excited about learning how to build our own apis