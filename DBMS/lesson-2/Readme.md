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

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20230920133529/onetoone.jpg"/>

### One-to-Many
 In one-to-many mapping as well where each entity can be related to more than one entity and the total number of tables that can be used in this is 2.

###  Many-to-Many
When entities in all entity sets can take part more than once in the relationship cardinality is many to many.

<img src="https://media.geeksforgeeks.org/wp-content/uploads/20230920133746/manytomany.jpg"/>








