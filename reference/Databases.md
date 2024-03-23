## Database Types

"The two types of databases in database management are operational databases and analytical databases."

Database Design for Mere Mortals, p4

### Analytical Databases

"... are primarily used in online analytical processing (OLAP) scenarios."

Database Design for Mere Mortals, p4

### Legacy Databases

"A legacy database is a database that has been in existence and in use for five years or more."

Database Design for Mere Mortals, p111

### Relational Database

"A relational database can be seen as a collection of organized and inter-related data on a related subject or topic."

Captain, Fidel A., Six-Step Relation Database Design, p2

## Database Normalization

"Normalization is the process of decomposing large tables into smaller ones in order to eliminate redundant data and duplicate data and avoid problems with inserting, updating, or deleting data."

Database Design for Mere Mortals, p26

### Other definition of normalization

"Normalization is the process of organizing the Relations (tables) in a database so that they reduce data redundancy and prevent inconsistent data dependencies."

Fidel A. Captain, Six-Step Relational Database Design, p166

### Database Normalization: Purpose

"[...] the purpose of normalization is to transform a set of improperly or poorly designed tables into tables with sound structures."

Database Design for Mere Mortals, p543

### Normal Form: Definition

"A normal form is a specific set of rules that can be used to test a table structure to ensure that it is sound and free of problems."

Database Design for Mere Mortals, p27

### Normalization is the test of good design

"Take a given table and test it agains normal forms to determine wether it is properly design."

Database Design for Mere Mortals, p543

#### First Normal Form (1NF)

"Any relation (table) that is first normal form exhibits domain integrity."

Fidel A. Captain, Six-Step Relational Database Design, p167

##### 1NF Result: Domain Integrity

"A domain is the set of all possible values of a given attribute, and domain integrity means that all the possible values of an attribute are legitimate ones."

Fidel A. Captain, Six-Step Relational Database Design, p167

#### Second Normal Form (2NF)

"Any table that is second normal form exhibits entity integrity and is also, by definition, it first normal form."

Fidel A. Captain, Six-Step Relational Database Design, p167

##### 2NF Result: Entity Integrity

"Entity integrity ensures that each row in the table is a unique and genuine entity, and that every other column in that table depends solely on the primary key."

Fidel A. Captain, Six-Step Relational Database Design, p167

#### Third Normal Form

"Any table that is in third normal form exhibits referential integrity and is also, by definition, in first and second normal forms."

Fidel A. Captain, Six-Step Relational Database Design, p167

##### 3NF Implementation

"A table should have a field that uniquely identifies each of its records, and each field in the table should describe the subject that the table represents."

Database Design for Mere Mortals, p27

##### 3NF Result: Referential Integrity

"Referential integrity is a characteristic of third normal form and ensures that foreign keys reference valid primary keys."

Fidel A. Captain, Six-Step Relational Database Design, p168

##### Referential Integrity: Definition

"Referential integrity ensures that all references to values in columns in other tables are authentic - authentic foreign key values."

Fidel A. Captain, Six-Step Relational Database Design, p167

##### 3NF is enough for most cases

"[...] Boyce-Codd Normal Form (BCNF), fourth, and fifth normal forms do exist, but 1NF, 2NF, and 3NF are usually sufficient to 'reduce data redundancy and prevent inconsistent data dependencies'."

Fidel A. Captain, Six-Step Relational Database Design, p167

## Database Keys

### Why keys are important

"They ensure that each record in a table is precisely identified."

Database Design for Mere Mortals, p234

### Keys help with integrity

"They [database keys] help establish and enforce various types of integrity."

Database Design for Mere Mortals, p234

### Key types

#### Candidate Key

"[A] candidate key, which is a field or a set of fields that uniquely identifies a single instance (a record in the table) of the table's subject."

Database Design for Mere Mortals, p235

##### A candidate key is a minimal superkey

"[...] if you remove any of the columns from the superkey, it won't be a superkey anymore."

Rod Stephens, Beginning Database Design Solutions, p53

#### Artificial Candidate Key

"When you determine that a table does not contain a candidate key, you can create and use an artificial (or surrogate) candidate key. (It's artificial in the sense that it didn't occur 'naturally' in the table; you have to manufacture it.)"

Database Design for Mere Mortals, p241.

#### Primary Key

##### Primary Key Field

"A primary key field exclusively identifies the table throughout the database structure and helps establish relationships with other tables."

Database Design for Mere Mortals, p243

##### Primary Key: role

"If you fail to assign a primary key to each table, you will eventually have data integrity problems."

Database Design for Mere Mortals, p201

##### Primary Keys are unique

"Each table must have one -and only one- primary key."

Database Design for Mere Mortals, p249

##### When primary keys are not 'unique'

"Each primary key within the database must be unique-no two tables should have the same primary key unless they bear a one-to-one relationship or one of them is a subset table."

Database Design for Mere Mortals, p249

##### Primary Key value

"A primary key value uniquely identifies a given record within a table and exclusively represents that record throughout the entire database. It also helps to guard agains duplicate records."

Database Design for Mere Mortals, p243

##### A primary key is a candidate key

"A primary key must conform to the exact same elements as a candidate key. This requirement is easy to fulfill because you select a primary key from a table's pool of available candidate keys."

Database Design for Mere Mortals, p243

##### Composite Primary Keys

"A primary key composed of two or more fields is known as a composite primary key."

Database Design for Mere Mortals, p248

## Database Table Types

### Data Table

"A table that stores data used to supply information is called a data table, and it is the most common type of table in a relation database."

Database Design for Mere Mortals, p42

### Validation Table

"A validation table (also known as a lookup table), on the other hand, stores data that you specifically use to implement data integrity."

Database Design for Mere Mortals, p43

### Linking Table

"You can establish the relationship via a set of primary and foreign keys [...] or through a third table known as a linking table (known as an associative table)."

Database Design for Mere Mortals, p51

#### When to use a linking table

"The best approach for you to take is to create and use a linking table, which will resolve the many-to-many relationship in the most appropriate and effective manner."

Database Design for Mere Mortals, p57

## Database Relationships

"[...] a relationship is defined as something that exists between entities."

Captain, Fidel A., Six-Step Relation Database Design, p38

### Degree of participation

"The degree of participation determines the minimum number of records that a given table must have associated with a single record in the related table, and the maximum number of records that a given table is allowed to have associated with a single record in the table."

Database Design for Mere Mortals

### Relationship types

#### Unary Relationship

"An unary relationship occurs when there are two entities involved in a relationship and they are the same entity."

Captain, Fidel A., Six-Step Relation Database Design, p38

#### Binary Relationship

"A binary relationship occurs when there are two entities involved in a relationship and the entities are different."

Captain, Fidel A., Six-Step Relation Database Design, p38

#### One-to-Many Relationship

##### One-to-Many Relationship: Purpose

"[...] it helps to eliminate duplicate data and to keep redundant data to an absolute minimum."

Database Design for Mere Mortals, p299

#### Self-Referencing Relationships

"A self-referencing relationship does not exist between a pair of tables [...]. It is instead a relationship that exists between the records within a table."

Database Design for Mere Mortals, p308

##### Self-Referencing One-to-One

"A self-referencing, one-to-one relationship exists when a given record in the table can be related to only one other record within the table."

Database Design for Mere Mortals, p309

##### Self-Referencing One-to-Many

"A table bears a self-referencing, one-to-many relationship to itself when a given record in the table can be related to one or more other records within a table."

Database Design for Mere Mortals, p309-310

##### Self-Referencing Many-to-Many

"A self-referencing, many-to-many relationship exists when a given record in the table can be related to one or more other records within the table and one or more records an themselves be related to the given record."

Database Design for Mere Mortals, p310

## Database Views

"[...] a view is a virtual table composed of fields from one or more tables in the database; it can also include fields from other views."

Database Design for Mere Mortals, p411

### Database Views: Anatomy

"You can define three types of view (data, aggregate, and validation) as you design the logical structure of the database and two types of views (materialized and partitioned) as you implement your database within an RDBMS."

Database Design for Mere Mortals, p413

### Views Are Dynamic

"The only information about a view that is stored in the database is its structure; the RBDMS rebuilds and "repopulates" the view every time you access the view in some manner."

Database Design for Mere Mortals, p411

### View Types

#### Validation View

"A validation view is similar to a validation table in that it can help implement data integrity."

Database Design for Mere Mortals, p422

##### Validation Views as Validation Tables

"You can define a validation view that works in the same manner as a validation table-its purpose is to provide a valid range of values for a given field in the database."

Database Design for Mere Mortals, p413

##### How to validate a field with a validation view

"When a business rule limits a particular field's range of values, you can enforce the constraint just as easily with a validation view as you can with a validation table."

Database Design for Mere Mortals, p422

#### Table View

"A view is a "virtual" table composed of fields from one or more tables in the database; the tables that comprise the view are known as base tables."

Database Design for Mere Mortals

#### Aggregate View

##### View Data is not modifiable

"Because an aggregate view is composed entirely of grouping fields and calculated fields, you cannot modify any of its data."

Database Design for Mere Mortals, p422

##### When to use a calculated field

"A good general rule to follow when you think you may need calculated fields is to use them if they will provide pertinent and meaningful information or if they will enhance the manner in which the view uses its data."

Database Design for Mere Mortals, p431

## Database Transaction

"A database transaction is a logical unit of database operations that are executed as one, all together or none at all."

Fidel A. Captain, Six-Step Relational Database Design, p163

### Transaction = consistency + reliability

"Each database transaction expects to find the database consistent and reliable state before it is processed and must leave the database in a consistent and reliable state for the next transaction."

Fidel A. Captain, Six-Step Relational Database Design, p163

### Transactions must be ACID

"Transactions must be Atomic, Consistent, Isolated and Durable (ACID)."

Fidel A. Captain, Six-Step Relational Database Design, p163

### Atomic transaction

"An _atomic transaction_ is a possibly complex series of actions that is considered as a single operation by those who are not involved directly in performing the transaction."

Rod Stephens, Beginning Database Design Solutions, p8

## Database Design

### Database Anti-Patterns

#### Jawwalking

"Programmers commonly use comma-separated lists to avoid creating an intersection table for a many-to-many relationship."

Bill Karwin, SQL Antipatterns, p13

#### Flat-File Design

"Flat-file design (sometimes known as the 'throw-everything-into-one-big-table') design."

Database Design for Mere Mortals, p456

##### Flat-File Design Problems

"[...] this structure will inevitably cause problems with redundant data and inconsistent data and that it suffers from a lack of data integrity."

Database Design for Mere Mortals, p456

## Database Refactoring

### Refactoring: Subset Tables

"Remove All the fields that the subset tables have in common and use them as the basis for a new data table."

Database Design for Mere Mortals, p220

## Database Replication

### Multi-master replication

"Instead of increasing the next ID by 1, we increase it by k, where k is the number of database servers in use."

Alex Xu, System Design Interview

#### Multi-master replication: drawbacks

- Hard to scale with multiple data centers
- IDs do not go up with time across multiple servers
- It does not scale well when a server is added or removed

Alex Xu, System Design Interview