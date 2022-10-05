# Readings: Mongo and Mongoose

## nosql vs sql

SQL
stands for Structured Query Language. It's used for relational databases. A SQL database is a collection of tables that stores a specific set of structured data.

NoSQL
are non-tabular databases and store data differently than relational tables. NoSQL databases come in a variety of types based on their data model. The main types are document, key-value, wide-column, and graph. They provide flexible schemas and scale easily with large amounts of data and high user loads.

(reference: https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)
## Questions 

1. Fill in the chart below with five differences between SQL and NoSQL databases:

SQL	NoSQL
- SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.
- SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. This means that SQL databases represent data in form of tables which consists of n number of rows of data whereas NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to.
- SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.
- SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable. SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load.
- SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful. In NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database.
 	 
2. What kind of data is a good fit for an SQL database?

table based data

3. Give a real world example.

Integrated Development Environment: Microsoft visual studio, Sql Server Management Studio and Visual Developer tools provide a very helpful way for development and increase the developers productivity.

4. What kind of data is a good fit a NoSQL database?

JSON

5. Give a real world example.

Speed: For simple queries, it gives good performance, as all the related data are in single document which eliminates the join operations; MongoDB

6. Which type of database is best for hierarchical data storage?

Redis

7. Which type of database is best for scalability?

MongoDB

## sql vs nosql (Video)

(reference: https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)
## Questions

1. What does SQL stand for?

Structured Query Language

2. What is a relational database?

is a database based on the relational model of data, as proposed by E. F. Codd in 1970. A system used to maintain relational databases is a relational database management system.

3. What type of structure does a relational database work with?

the data tables, views, and indexes

4. What is a ‘schema’?

A database schema is considered the “blueprint” of a database which describes how the data may relate to other tables or other data models.

5. What is a NoSQL database?

 provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases.

6. How does it work?

allow developers to store huge amounts of unstructured data, giving them a lot of flexibility.

7. What is inside of a Mongo database?

a database contains the collections of documents

8. Which is more flexible - SQL or MongoDB? and why.

MongoDB more flexible; MongoDB's collections, by default, do not require their documents to have the same schema

9. What is the disadvantage of a NoSQL database?

Compatibility issues with SQL instructions. New databases use their own characteristics in the query language and they're not yet 100% compatible with the SQL used in relational databases. 

## Things I want to Know more about 