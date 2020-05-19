# Advanced Mongo/Mongoose

- 1. Why would a developer choose to make data models?
  - Models promote consensus among developers, customers and other stakeholders. A data model also promotes agreement on vocabulary and jargon. The model highlights the chosen terms so that they can be driven forward into software artifacts. The resulting software becomes easier to maintain and extend

- 2. What purpose do CRUD operations serve?
  - This helps making every id in the context data unique. CREATE a new entity and add to the context. CREATE or UPDATE an attribute of a specified entity. READ entity data from the context.

- 3. What kind of database is Postgres? What kind of database is MongoDB?
  - PostgreSQL is a relational database management system. 
  - MongoDB is an open source, non- relational database management system. 


- 4. What is Mongoose and why do we need it?
  - Mongoose is an Object Data Modeling (ODM) library for MongoDB and Node. js. It manages relationships between data, provides schema validation, and is used to translate between objects in code and the representation of those objects in MongoDB.


- 5. Describe how NoSQL Databases scale horizontally
  -  NoSQL databases are designed to expand horizontally and in Horizontal scaling means that you scale by adding more machines into your pool of resources.


- 6. Give one strong argument for and against NoSQL Databases
  - JOINs are important because they allow you to maintain a single source of truth and access disparate data easily.
  - OIN allows me to connect any piece of data in the DB to any other related piece of data by simply connecting the tables. This means that I can create a fully normalized structure and store each piece of data exactly once in exactly one place. i.e. a fully normalized database


- 7. Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.
  - Constraints are a very important feature in a relational model. In fact, the relational model supports the well-defined theory of constraints on attributes or tables. Constraints are useful because they allow a designer to specify the semantics of data in the database. Constraints are the rules that force DBMSs to check that data satisfies the semantics.
  - Domain Integrity,Entity integrity,Referential integrity.


- 8. Name 3 cloud based NoSQL Databases
  - Redis is an open source in-memory data structure server and NoSQL database.
  - Couchbase headquartered in Mountain View, California offers the Couchbase Server, a NoSQL database.
  - Cassandra is a no-SQL database from Apache.



  ## Vocabulary Terms
  
Vocabulary                   |  Definition
-----------------------------|----------------------------------------------------------------------------------------------------
database                     | is an organized collection of structured information, or data, typically stored electronically in a                                       computer system.
  data model                     | define how data is connected to each other and how they are processed and stored inside the system.
  CRUD                           | represents an acronym for the database operations Create, Read, Update, and Delete.
  schema                         | is a collection of database objects including tables, views, triggers, stored procedures, indexes, etc.
  sanitize                       | means that you remove all dangerous characters from an input string before passing it to the SQL engine.                                                                       
  Structured Query Language (SQL)| is a programming nomenclature used to do set operations (like union, intersect, and minus) to organize and retrieve information in relational databases, based on “set theory and relational algebra.                   
  Non SQL (NoSQL)                | database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases.   
  MongoDB                        |  is one of the most popular document based NoSQL database as it stores data in JSON like documents. It is non-relational database with dynamic schema.
  Mongoose                       | is an Object Data Modeling (ODM) library for MongoDB and Node. ... MongoDB is a schema-less NoSQL document database. It means you can store JSON documents in it, and the structure of these documents can vary as it is not enforced like SQL databases.
  record                         | is a group of related data held within the same structure. 
  document                       | is a type of nonrelational database that is designed to store and query data as JSON-like documents.
  Object Relation Mapping (ORM)  | in computer science is a programming technique for converting data between incompatible type systems using object-oriented programming languages.



# In Memory Database Testing
## Testing Node.js + Mongoose with an in-memory database

   - In-memory database pros & cons
     - **Pros:**
       - No need for mocks
       - Faster development
       - More reliable tests
       - Tests are easier to build

     - **Cons:**
       - The in-memory database probably needs seeding
       - More memory usage (dah)
       - Tests take longer to run (depending on your hardware).

# The Repository Design Pattern
  - the important thing you must remember is that design patterns do not depend on specific technology, framework or programming language.
  -  A design pattern is not a design which is directly transferred into code(source or machine).
  - Repository pattern separates the data access logic and maps it to the business entities in the business logic.
  - Communication between the data access logic and the business logic  is done through interfaces.

  - **The separation of data access from business logic have many benefits. Some of them are:**
    - Centralization of the data access logic makes code easier to maintain
    - Business and data access logic can be tested separately
    - Reduces duplication of code
    - A lower chance for making programming errors
