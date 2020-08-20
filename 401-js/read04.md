# Read: 04 - Advanced Mongo/Mongoose


[README](/README.md)


## Research Questions:

Why would a developer choose to make data models? resources: [bridging the gap](https://www.bridging-the-gap.com/3-reasons-to-data-model/)
- data models are easier to change than databases -- lets all parties involved explore the data paths that are needed and be able to discuss exactly what the end product will eventually look like
  - we can delete fields that we do not want prior to building the db
  - you can change attributes and anything else

What purpose do CRUD operations serve? [Create, read, update and delete](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete)
- CRUD operations allow the application to be useable. 
- CREATE or add new entries;
- READ retrieve, search, or view existing entries;
- UPDATE or edit existing entries;
- DELETE, deactivate, or remove existing entries.

 What kind of database is Postgres? What kind of database is MongoDB?
- Postgres is a relational db
- MongoDB is schema-less, it  is documented based which uses collections to store the related information. 
- PostgreSQL is used mainly when static JSON is used and data is structured for SQL storage. 
- MongoDB is mainly used when data is unstructured and there is a need for modifying the JSON data inside the storage.


What is Mongoose and why do we need it?
  - See below. 

- Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.



<br>
<br>
<br>
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

<br>
<br>
<br>

# Additional Readings

## [External ARTICLE: Testing Node.js + Mongoose with an in-memory database](https://dev.to/paulasantamaria/testing-node-js-mongoose-with-an-in-memory-database-32np)

mongodb-memory-server
  -  allows us to start a mongod process that stores the data in memory.
  - used instead of needing logic for mocks
    - Database Mocking --- bMocking database is a technique that allows you to set the desired database state (for different tables) in your tests to let specific data-sets ready for future test execution.

### In-memory db pros and cons
Pros
  - no need for mocks: code is directly executed using the in memory db
  - faster development 
  More reliable tests: using this technology, you are testing the actual cod e that will be executed on production instead of with mock that may not be accurate or up to date
  - tests are easier to build! ? 

Cons
- in memory db needs seeding?
- more memory usage
- tests take longer to run... 
# Reference the ABOVE article for setting up in-memory dbs!


## [External ARTICLE: The Repository Design Pattern](https://cubettech.com/resources/blog/introduction-to-repository-design-pattern/)
Repository pattern
- is a kind of container where data access logic is stored. It hides the details of data access logic from business logic. In other words, we allow business logic to access the data object without having knowledge of underlying data access architecture.
  - makes code easier to maintain
  - busines and data logic can be tested seperately
  -reduces duplication of code
  - low chance for making programming errors


## [External ARTICLE: github README: MongoDB In-Memory Server](https://github.com/nodkz/mongodb-memory-server)
This package spins up a real honest to god MongoDb server PROGRAMATICALly from node.
- used for testing or mocking during development 
There are three packages all for different purposes ---that being said, they are the same apart from default configurations
- mongodb-memory-server, mongodb-memory-server-global, mongodb-momory-server-core
