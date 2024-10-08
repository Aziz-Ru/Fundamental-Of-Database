# Introduction of ER Model

The Entity Relational Model is a model for identifying entities to be represented in the database and representation of how those entities are related. The overall logical structure (schema) of a database can be expressed graphically by an entity-relationship (E-R) diagram.

## Symbols Used in ER Model 

- Rectangles: _Rectangles represent Entities in the ER Model._
- Ellipses: _Ellipses represent Attributes in the ER Model._
- Diamond: _Diamonds represent Relationships among Entities._
- Lines: _Lines represent attributes to entities and entity sets with other relationship types._
- Double Ellipse: _Double Ellipses represent Multi-Valued Attributes._
- Double Rectangle: _Double Rectangle represents a Weak Entity._

##
  <img src="https://media.geeksforgeeks.org/wp-content/uploads/20230428115454/Introduction-to-ER-Model-2-768.webp"/>

## Components of ER Diagram 

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20230428090323/Introduction-to-ER-Model-1-768.webp"/>


### Entity
An entity is a “thing” or “object” in the real world that is distinguishable from other objects.
An entity set is a set of entities of the same type that share the same properties,or attributes.

#### Strong Entity 
A Strong Entity is a type of entity that has a key Attribute. Strong Entity does not depend on other Entity in the Schema. It has a primary key, that helps in identifying it uniquely, and it is represented by a rectangle. 

#### Weak Entity 
An Entity type has a key attribute that uniquely identifies each entity in the entity set. But some entity type exists for which key attributes can’t be defined. These are called Weak Entity types . A weak entity type is represented by a Double Rectangle

###  What is Attributes?

Attributes are the properties that define the entity type. an attribute is a piece of data that describes an entity

 #### Key Attribute
The attribute which uniquely identifies each entity in the entity set is called the key attribute.
<img src="https://media.geeksforgeeks.org/wp-content/uploads/Database-Management-System-ER-Model-3.png"/>

### Composite Attribute
An attribute composed of many other attributes is called a composite attribute.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/Database-Management-System-ER-Model-4.png"/>

### Multivalued Attribute
  An attribute consisting of more than one value for a given entity.In ER diagram, a multivalued attribute is represented by a double oval. 
<img src="https://media.geeksforgeeks.org/wp-content/uploads/Database-Management-System-ER-Model-5.png"/>

 ### Derived Attribute

An attribute that can be derived from other attributes of the entity type is known as a derived attribute. In ER diagram, the derived attribute is represented by a dashed oval. 

<img src="https://media.geeksforgeeks.org/wp-content/uploads/Database-Management-System-ER-Model-6.png"/>

### Descriptive attributes
A relationship may also have attributes called descriptive attributes

## Degree of a Relationship Set
_The number of different entity sets participating in a relationship set is called the degree of a relationship set._

### Unary Relationship
When there is only ONE entity set participating in a relation, the relationship is called a unary relationship. For example, one person is married to only one person. 

### Binary Relationship
 When there are TWO entities set participating in a relationship, the relationship is called a binary relationship.
<img src="https://media.geeksforgeeks.org/wp-content/uploads/Database-Management-System-ER-Model-8.png"/>

 ### Ternary Relationship
 When there are three entity sets participating in a relationship, the relationship is called a ternary relationship. 

## What is Cardinality? 
_The number of times an entity of an entity set participates in a relationship set is known as cardinality ._

### One-to-One
When each entity in each entity set can take part only once in the relationship, the cardinality is one-to-one.the total number of tables that can be used in this is 2. 
If conver this ER model to Relational Model we get 3 table two for entites ans 1 for relation. in relation table any primary key can be a rimary key. if we minimize this we need 2 table
bacause if we merge on table pk to another table.
<img src="https://media.geeksforgeeks.org/wp-content/uploads/20230920133529/onetoone.jpg"/>

### One-to-Many
 In one-to-many mapping as well where each entity can be related to more than one entity and the total number of tables that can be used in this is 2.First if we convert relational table we get 3 table. If we merge with pk which is many we solve this in 2 table.

###  Many-to-Many
When entities in all entity sets can take part more than once in the relationship cardinality is many to many.we cannot minimize table so that we need 3 atble.Relation table primary key is composite of two pk, because multiple primary key.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20230920133746/manytomany.jpg"/>

## Participation Constraints in ER-Model
Participation Constraints tell us that the participation in a relationship can either be total or partial. 

### Total Participation

When each entity in an entity set participates in a relation, it is called Total Participation. 

### Partial Participation

When all entities in the given entity set do not participate in a relation, it is called Partial Participation. 

## Generalization, Specialization and Aggregation in ER Model

### Generalization
Generalization is the process of extracting common properties from a set of entities and creating a generalized entity from it. 

### Specialization
In specialization, an entity is divided into sub-entities based on its characteristics. It is a top-down approach where the higher-level entity is specialized into two or more lower-level entities.



### Aggregation
Aggregation in DBMS(Database Management System) is a process of combining two or more entities to form a more meaningful entity.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20230612113346/aggregation.webp"/>

## Reduction of ER diagram to Table

There are some points for converting the ER diagram to the table:
- Entity type becomes a table.
- All single-valued attribute becomes a column for the table.
- A key attribute of the entity type represented by the primary key
- The multivalued attribute is represented by a separate table.
- Composite attribute represented by components.
- Derived attributes are not considered in the table

Way
- Identify each distinct entity in the diagram represented by a rectangle.
- Create Separate Tables for Each Entity
- Map Relationships
        - For one-to-many relationships, add a foreign key in the “many” table referencing the “one” table’s primary key.
        - For many-to-many, create a linking table with foreign keys to both related tables.

### To Minimize ER Diagram

- 1 to m or m to 1 relations combine entity and relation which is many,so we need only two table.
- m to n relation there need 3 table .
- 
- [Mapping from ER Model to Relational Model](https://www.geeksforgeeks.org/mapping-from-er-model-to-relational-model/)
- [Problems](https://www.gatevidyalay.com/er-diagrams-to-tables/)



