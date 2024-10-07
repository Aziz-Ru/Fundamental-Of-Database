# Introduction of DBMS

## What is DBMS?

A Database Management System (DBMS) is a software system that is designed to manage and organize data in a structured manner.It allows users to create, modify, and query a database, as well as manage the security and access controls for that database.
_The primary goal of a DBMS is to provide a way to store and retrieve database information that is both convenient and efficient_

## Key Features of DBMS

- Data modeling: A DBMS provides tools for creating and modifying data models, which define the structure and relationships of the data in a database.
- Data storage and retrieval: A DBMS is responsible for storing and retrieving data from the database, and can provide various methods for searching and querying the data.
- Concurrency control: A DBMS provides mechanisms for controlling concurrent access to the database, to ensure that multiple users can access the data without conflicting with each other.
- Data integrity and security: A DBMS provides tools for enforcing data integrity and security constraints, such as constraints on the values of data and access controls that restrict who can access the data.
- Backup and recovery: A DBMS provides mechanisms for backing up and recovering the data in the event of a system failure.

## Database Languages
- ### Data Definition Language
- ### Data Manipulation Language
- ### Data Control Language
- ### Transactional Control Language

## Data Definition Language (DDL)

DDL is the short name for Data Definition Language, which deals with database schemas and descriptions, of how the data should reside in the database.

- CREATE: to create a database and its objects like (table, index, views, store procedure, function, and triggers)
- ALTER: alters the structure of the existing database
- DROP: delete objects from the database
- TRUNCATE: remove all records from a table, including all spaces allocated for the records are removed
- COMMENT: add comments to the data dictionary
- RENAME: rename an object

## Data Manipulation Language (DML)

DML is the short name for Data Manipulation Language which deals with data manipulation and includes most common SQL statements such SELECT, INSERT, UPDATE, DELETE, etc., 
and it is used to store, modify, retrieve, delete and update data in a database.

    - SELECT: retrieve data from a database
    - INSERT: insert data into a table
    - UPDATE: updates existing data within a table
    - DELETE: Delete all records from a database table
    - MERGE: UPSERT operation (insert or update)
    - CALL: call a PL/SQL or Java subprogram
    - EXPLAIN PLAN: interpretation of the data access path
    - LOCK TABLE: concurrency Control


## Data Control Language (DCL)

DCL is short for Data Control Language which acts as an access specifier to the database.(basically to grant and revoke permissions to users in the database

  - GRANT: grant permissions to the user for running DML(SELECT, INSERT, DELETE,…) commands on the table
  - REVOKE: revoke permissions to the user for running DML(SELECT, INSERT, DELETE,…) command on the specified table

## Transactional Control Language (TCL)

TCL is short for Transactional Control Language which acts as an manager for all types of transactional data and all transactions. Some of the command of TCL are

   - Roll Back: Used to cancel  or Undo changes made in the database 
   - Commit: It is used to apply or save changes in the database
   - Save Point: It is used to save the data on the temporary basis in the database

## Disadvantage of File System

- Redundancy of data: Data is said to be redundant if the same data is copied at many places.
- No abstraction: The file system is not provide users with an abstract view of the data
- Inconsistency of Data: Data is said to be inconsistent if multiple copies of the same data do not match each other.
- Difficult Data Access: A user should know the exact location of the file to access data, so the process is very cumbersome and tedious.
- Unauthorized Access: File Systems may lead to unauthorized access to data.
- No Concurrent Access: The access of the same data by multiple users at the same time is known as concurrency.
- No Backup and Recovery: The file system does not incorporate any backup and recovery of data if a file is lost or corrupted.
- Integrity problems. The data values stored in the database must satisfy certain types of consistency constraints.

## Data Abstraction
Data Abstraction in Database Management Systems (DBMS) is a concept that hides the complexity of the database from the user by providing a simplified view.

### Physical level
The lowest level of abstraction describes how the data are actually stored.

### Logical level
The next-higher level of abstraction describes what data are stored in the database, and what relationships exist among those data.
### View level
The highest level of abstraction describes only part of the entire database.

## Types of DBMS Architecture

- 1-Tier Architecture
- 2-Tier Architecture
- 3-Tier Architecture

## 1-Tier Architecture
In 1-Tier Architecture the database is directly available to the user, the user can directly sit on the DBMS and use it that is, the client, server, and Database are all present on the same machine.

##  2-Tier Architecture

The 2-tier architecture is similar to a basic client-server model . The application at the client end directly communicates with the database on the server side.

##  3-Tier Architecture

In 3-Tier Architecture , there is another layer between the client and the server. The client does not directly communicate with the server. Instead, it interacts with an application server which further communicates with the database system and then the query processing and transaction management takes place.

## Schema and Instance
- Instance:The collection of information stored in the database at a particular moment is called an instanceof the database.
- Schema:The overall design of the database is called the database schema.
