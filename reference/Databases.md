### Database Purpose

"Every database is created for a specific purpose, wether it's to solve a particular business problem, to manage the daily transactions of a business or organization, or to be used as a part of an information system."

Database Design for Mere Mortals, p69-70

### Database Goal

"The database supports business rules relevant to the organization. The. data must provide valid and accurate information that is always meaningful to the business."

Database Design for Mere Mortals, p23

### The goal of a Database Architect

"Your goal as the database architect is to make certain that it has only an *absolute minimum* amount of redundant data."

Database Design for Mere Mortals, p206

## Database Mission Statement

"The mission statement establishes the purpose of the database and provides you with a distinct  focus for your design work."

Database Design for Mere Mortals, p69

### Mission Statement: Creation Process

"The process of creating a mission statement involves conducting an interview with the owner or manager of the organization, learning about the organization, and determining the purpose of the new database."

Database Design for Mere Mortals, p93

### Database Statement: Mission Objectives

"... are statements that represent the general tasks supported by the data maintained in the database."

Database Design for Mere Mortals, p96

#### Well written mission objectives

"Each mission objective represents a single general task and define the task clearly without unnecessary details."

Database Design for Mere Mortals, p97

### When the mission statement is wrong

"The specific purpose of the database is unclear. This mission statement is written in such a way that ascertaining the specific purpose of the database is difficult."

### When the mission statement is complete

"Your mission statement is complete when you have a sentence that describes the specific purpose of the database and that is understood and agreed upon by everyone concerned."

Database Design for Mere Mortals, p94

## Database Data

### Data: definition

"The values you store in the database are data. Data is static in the sense that it remains in the same state until you modify it by some manual or automated process."

Database Design for Mere Mortals, p35

#### What data to store

"you wouldn't necessarily want or need to store very last piece of data the organization migh possibly use. The data you finally choose to store and how you decide to store it will be determined by the way the organization uses its data."

Database Design for Mere Mortals, p370

### Data Integrity

"... refers to the validity, consistency, and accuracy of the data in a database."

Database Design for Mere Mortals, p59

#### Data Integrity: Importance

"Unless the database stores its data safely and effectively, the application will be useless no matter how well-designed the rest of the system may be."

Rod Stephens, Beginning Database Design Solutions, pXXV

"[...] a crack in the integrity could result in inconsistent data or inaccurate information."

Database Design for Mere Mortals, p446

#### Data Integrity vs Performance

"Any time you break the rules for the sake of performance (or any other reason, for that matter), you are surely going to introduce data-integrity problems."

Database Design for Mere Mortals, p467

### Data Consistency

"Consistency means different parts of the database don't hold contradictory views on the same information."

Rod Stephens, Beginning Database Design Solutions, p10

### Data Validity

"Validity mean data is validated where possible against other pieces of data in the database."

Rod Stephens, Beginning Database Design Solutions, p10

### Consequences of poor data

"[...] even if the application is well designed, poor data design will inevitably result in a poor application."

Captain, Fidel A., Six-Step Relation Database Design, p xvii-xviii

### Redundant Data

"Redundant data is a value that is repeated in a field as a result of the field's participation in relating two tables or as a result of some field or table anomaly."

Database Design for Mere Mortals, p208

### Information

"Information is data that you process in a manner that makes it meaningful and useful to you when you work with it or view it."

Database Design for Mere Mortals, p35

#### The problem with inaccurate information

"Inaccurate information is probably the most detrimental result of improper database design - it can adversely affect your organization's bottom line."

Database Design for Mere Mortals, p18

### Data vs Information

"The point to remember is that you must process your data in some manner so that you can turn it into meaningful information."

Database Design for Mere Mortals, p35

### Data vs Information: other definition

"Data is what you store, information is what you retrieve."

Database Design for Mere Mortals, p36



## Database Types

"The two types of databases in database management are operational databases and analytical databases."

Database Design for Mere Mortals, p4

### Paper-based databases

"This type of database typically contains inconsistent data, erroneous data, duplicate data, redundant data, incomplete entries, and old data that should have been purged from the database long ago."

Database Design for Merge Mortals, p111

### Operational Databases

"This type of database if primarily used to collect, modify, and maintain data on a da-to-day basis. The type of data stored is _dynamic_, meaning that it changes constantly and always reflects up-to-the-minute information"

John L. Viescas, SQL for mere mortals, p16

#### Operational Databases: Usages

"Operational databases [are] primarily used in online transaction processing (OTPL) scenarios"

Database Design for Mere Mortals, p4

### Analytical Databases

"... are primarily used in online analytical processing (OLAP) scenarios."

Database Design for Mere Mortals, p4

"an analytical database stores and tracks historical and time-dependent data."

John L. Viescas, SQL for mere mortals, p

#### Analytical Databases are derived from operational databases

"Note that the data found in analytical databases is usually gleaned from an operational database."

John L. Viescas, SQL for mere mortals, p16

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

#### Super Key

"A _superkey_ is a set of one or more columns in a table for which no two rows can have the exact same values."

Rod Stephens, Beginning Database Design Solutions, p53

#### Candidate Key

"[A] candidate key, which is a field or a set of fields that uniquely identifies a single instance (a record in the table) of the table's subject."

Database Design for Mere Mortals, p235

##### A candidate key is a minimal superkey

"[...] if you remove any of the columns from the superkey, it won't be a superkey anymore."

Rod Stephens, Beginning Database Design Solutions, p53

##### Candidate Key vs Unique Key

"A _unique key_ is a superkey that is used to uniquely identify the rows in a table. The difference between a unique key and any other candidate key is in how it is used. A candidate key _could_ be used to identify rows if you wanted it to, but a unique key is used to constraint the data."

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

### Subset tables

"Tables that have almost identical structures are commonly subset tables; there are usually only a few unique fields that distinguish one table from the other."

### Validation Table

"A validation table (also known as a lookup table), on the other hand, stores data that you specifically use to implement data integrity."

Database Design for Mere Mortals, p43

### Linking Table

"You can establish the relationship via a set of primary and foreign keys [...] or through a third table known as a linking table (known as an associative table)."

Database Design for Mere Mortals, p51

#### When to use a linking table

"The best approach for you to take is to create and use a linking table, which will resolve the many-to-many relationship in the most appropriate and effective manner."

Database Design for Mere Mortals, p57


## Database Columns

"a column represents a characteristic of the subject of the table to which it belongs to."

John L. Viescas, SQL for mere mortals, p35

### Column Domain

"The set of values that are allowed for a column is called the column's _domain_."

Rod Stephens, Beginning Database Design Solutions, p50


## Database Relationships

"[...] a relationship is defined as something that exists between entities."

Captain, Fidel A., Six-Step Relation Database Design, p38

### Degree of participation

"The degree of participation determines the minimum number of records that a given table must have associated with a single record in the related table, and the maximum number of records that a given table is allowed to have associated with a single record in the table."

Database Design for Mere Mortals

### Table Participation

"A table's participation within a relationship can be either mandatory or optional."

Database Design for Mere Mortals, p57

### Cardinality

"Cardinality indicates the number of entity occurrences in a relationship, which can be any number from zero to infinity."

Captain, Fidel A., Six-Step Relation Database Design, p67

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





## Database Associations

### Reflexive / Recursive Association

"A _reflexive_ or _recursive_ association is one in which an object refers to an object of the same class."

Rod Stephens, Beginning Database Design Solutions, p193

### Multiple-Object Association

"A multiple-object association is one where many different kinds of objects are collectively associated to each other."

Rod Stephens, Beginning Database Design Solutions, p188


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

#### Importance of ACID transactions

"ACID compliance guarantees the integrity of the data in the tables of an RDBMS database each time a database transaction is processed."

Fidel A. Captain, Six-Step Relational Database Design, p163

### Atomic transaction

"An _atomic transaction_ is a possibly complex series of actions that is considered as a single operation by those who are not involved directly in performing the transaction."

Rod Stephens, Beginning Database Design Solutions, p8



## Database Design

### Database Design is not "simple"

"Simple is one of the most dangerous words known to database developers. Nothing is ever 'simple'."

Database Design for Mere Mortals, p68

### Traditional phases of database design

"In general, traditional methods of database design incorporate three phases: requirement analysis, data modeling, and normalization."

Database Design for Mere Mortals, p24

### Logical Database Design

"The logical database design describes the size, shape, and necessary systems for our database, and it addresses the informational and operational needs of your business."

Database Design for Mere Mortals, p19.

### Physical vs Logical Design

"You should always design the logical structure of your database without regard to any RDBMS . By doing so, you're more likely to design a sound structure because you'll be focused on the organization's information requirements."

Database Design for Mere Mortals, p462

#### Separate Logical and Physical Design

"[...] the logical design process and the physical design and implementation process should be kept separate."

Database design for Mere Mortals, p548

##### What happens if you don't separate logical from physical design

"Using this approach to design a database commonly results in improper structural design, insufficient data integrity, and problems with inconsistent data and inaccurate information."

Database Design for Mere Mortals, p549

#### Database Design should dictate RDBMs, not the other way around

"I believe you should always design the logical structure of you database without regard to any RDBMS. By doing so, you're more likely to design a sound structure because you'll be focused on the organization's information requirements. After your design is complete, you can then clearly determine how you should implement the database (single-user application, client/server, web-based, and so on) and which RDBMS you should use to facilitate the implementation."

Database Design for Mere Mortals, p549

##### RMDBs will influence your design choices

"Your design will be constrained by your knowledge of the RDBMS. For example, you may decide not to implement relationship characteristics simply because you don't know how to do so."

Database Design for Mere Mortals, p462

"You'll inadvertently let the RDBMS dictate the design of the database as opposed to driving the design strictly from organization's information requirements."

Database Design for Mere Mortals, p549

### Conceptual Models

"Conceptual models are concerned with the logical nature of the data and what is represented."

Captain, Fidel A., Six-Step Relation Database Design, p6

#### Conceptual Model's Concerns

"Conceptual models are concerned with the logical nature of the data and what is being represented."

Captain, Fidel A., Six-Step Relation Database Design, p94

#### Entity-Relationship Model

"The E-R diagram is a conceptual model and represents the user's view of the datad and the logical structure of the database."

Captain, Fidel A., Six-Step Relation Database Design, p94

### Implementation Models

"[...] implementation models are concerned with the physical nature of the data and with how the data will be represented in the database."

Captain, Fidel A., Six-Step Relation Database Design, p6

#### Implementation Model's Concerns

"[...] implementation models are concerned with the physical nature of the data and with how the data will be represented in the database."

Captain, Fidel A., Six-Step Relation Database Design, p94

#### Relation-Model Diagrams

"[...] the R-M diagram is an implementation model and represents the developer's view of the data and the physical structure of the database."

Captain, Fidel A., Six-Step Relation Database Design, p94

### E-R Diagrams vs R-M diagrams

"The E-R diagram is a conceptual model and the R-M diagram is an implementation model."

Captain, Fidel A., Six-Step Relation Database Design, p94

### Conceptual vs Implementation Models

"Generally, conceptual models are concerned with the user's view of the data, and implementation models are concerned with the developer's view of the data."

Captain, Fidel A., Six-Step Relation Database Design, p6

### Field Design

#### Fields are singular

"Words that identify fields are always singular ('Home Phone', not 'Home Phones'). Following this rule will make it easy for you to differentiate between table names and field names in any documentation you create for the database."

Database Design for Mere Mortals, p181

#### Field design is dictated by the purpose of the data

"Defining field specifications compels you to acquire a complete understanding of the nature and purpose of the data in the database."

Database Design for Mere Mortals, p265

#### Meaning of null

"Null does not represent a blank - it represents a missing or unknown value."

Database Design for Mere Mortals, p279

### Attribute Design

"Attributes should represent one and only one characteristic or property of an entity. They should not represent multiple characteristics or properties."

Captain, Fidel A., Six-Step Relation Database Design, p22

### Table Design

#### Why table names are plural

"You use the plural form because a table stores a _collection of instances_ of the subject of the table."

John L. Viescas, SQL for mere mortals, p48

### Column Design

### Cascade Updates

"Cascade updates ensures referential integrity by updating all references to a primary key value which has changed, by updating all corresponding foreign key values for that primary key."

Fidel A. Captain, Six-Step Relational Database Design, p168

#### Deletion Rule

"You always set the deletion rule from the perspective of the parent table because it is the more important of the two tables within the relationship. Deleting a record in the parent table will always have some effect on related records in the child table, but deleting a record in the child table will have little if any effect on the related record in the parent table."

Database Design for Mere Mortals, p353

### Database Anti-Patterns

#### Tables with ambiguous names

"A table with an ambiguous name suggests that you may not have identified the subject clearly or accurately during the analysis and interview process."

Database Design for Mere Mortals, p180

#### Dependent table descriptions

"Do no make the table description for one table dependent upon the table description of another table. Each table description should be self-explanatory and independent from every other table description."

Database Design for Mere Mortals, p185

#### Jaywalking

"Programmers commonly use comma-separated lists to avoid creating an intersection table for a many-to-many relationship."

Bill Karwin, SQL Antipatterns, p13

#### Flat-File Design

"Flat-file design (sometimes known as the 'throw-everything-into-one-big-table') design."

Database Design for Mere Mortals, p456

##### Flat-File Design Problems

"[...] this structure will inevitably cause problems with redundant data and inconsistent data and that it suffers from a lack of data integrity."

Database Design for Mere Mortals, p456

### Start Database Designs from Scratch

"Do not adopt the current database structure as the basis for the new database structure."

Database Design for Mere Mortals, p110

## Database Refactoring

### Refactoring: Subset Tables

"Remove All the fields that the subset tables have in common and use them as the basis for a new data table."

Database Design for Mere Mortals, p220


## Database Replication

### Master-Slave Benefit: better performance

"This model improves performance because it allows more queries to be processed in parallel."

Alex Xu, System Design Interview

### Master Slave Benefit: High Availability

"By replicating data across different locations, your website remains in operation even if a database is offline as you can access data stored in another database server."

Alex Xu, System Design Interview

### Master-Slave Reliability

"You do not need to worry about data loss because data is replicated across multiple locations."

Alex Xu, System Design Interview

### Master-Slave Ratio

"Most applications require a much higher ratio of reads to writes; thus, the number of slave databases in a system is usually larger than the number of master databases."

Alex Xu, System Design Interview

### What if the master database goes offline?

"If the master database goes offline, a slave database will be promoted to be the new master. All database operations will be temporarily executed on the new master database."

Alex Xu, System Design Interview

### What if the slave database goes offilne?

"If only one slave database is available and it goes offline, read operations will be redirected to the master database temporarily."

Alex Xu, System Design Interview

### Master Database Allowed Operations

"A master database generally only supports write operations."

Alex Xu, System Design Interview

### Slave database allowed operations

"A slave database gets copies of the data from the master database and only supports read operations."

Alex Xu, System Design Interview

### Multi-master replication

"Instead of increasing the next ID by 1, we increase it by k, where k is the number of database servers in use."

Alex Xu, System Design Interview

#### Multi-master replication: drawbacks

- Hard to scale with multiple data centers
- IDs do not go up with time across multiple servers
- It does not scale well when a server is added or removed

Alex Xu, System Design Interview
