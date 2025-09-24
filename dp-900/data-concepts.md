# Data Concepts 


## The concepts of relational and non-relational data.

### Relational data
Relational data is structured data that follows a tabular format — like rows and columns in a table — and is stored in Relational Database Management Systems (RDBMS).

### Non Relational data
Non-relational data does not use tables to store information. Instead, it uses formats like documents, key-value pairs, graphs, or wide-column stores. These are stored in NoSQL databases.

- test
- test1
##Data can be classified as structured, semi-structured, or unstructured.

### Structured data - 
Structured data - adheres to a fixed schema, in tabular format , has the same fields or properties.
### Semi-structured data -
is information that has some structure, but which allows for some variation between entity instances. e.g. JSON
### Unstructured data -
documents, images, audio and video data, and binary files might not have a specific structure. This kind of data is referred to as unstructured data.

### Data store:
Organizations typically store data in structured, semi-structured, or unstructured format 
There are two broad categories of data store in common use:
- File stores
- Databases

### Differnt types of file staorage
- **Delimited text files**: Data is often stored in plain text format with specific field delimiters and row terminators. Ex: CSV(comma seperated), TSV(tab seperated or space seperated). Good choice for structured data
- **JavaScript Object Notation (JSON)**: JSON is a ubiquitous format in which a hierarchical document schema is used to define data entities (objects) that have multiple attributes. Good for both structured and semi-structured data.
- **XML**
- **Binary Large Object (BLOB)**: for unstructured data, store the data as raw binary that must be interpreted by applications and rendered. EX. Common types of data stored as binary include images, video, audio, and application-specific documents.
- **Optimized file formats**: specialized file formats that enable compression, indexing, and efficient storage and processing have been developed.
  - **Avro**: row-based format. Avro is a good format for compressing data and minimizing storage and network bandwidth requirements.
  - **ORC** (Optimized Row Columnar format): organizes data into columns rather than rows. Used for optimizing read and write operations in Apache Hive (Hive is a data warehouse system that supports fast data summarization and querying over large datasets)
  - **Parquet**: is another columnar data format: is columnar data format. Parquet specializes in storing and processing nested data types efficiently. It supports very efficient compression and encoding schemes. A Parquet file contains row groups. 

### Explore Databases
A database is used to define a central system in which data can be stored and queried
  - **Relational databases**: Relational databases are commonly used to store and query structured data.  Use of keys to reference data entities enables a relational database  to be normalized; which in part means the elimination of duplicate data values is called normalisation
  - **Non-relational databases**: Non-relational databases are data management systems that don’t apply a relational schema to the data. Non-relational databases are often referred to as NoSQL database, even though some support a variant of the SQL language.
        **Four common types of Non-relational database commonly in use**:
        Key-value databases,
        Document databases,
        Column family databases,
        Graph databases

### Transactional data processing
A transactional data processing system is a computer system that records important business events, like money transfers in a bank or payments in a store. Each transaction is a small, separate piece of work that the system keeps track of.

OLTP systems use databases designed for fast reading and writing of data. They handle day-to-day business transactions (create, read, update, delete – CRUD) while keeping data accurate and safe through ACID rules:
 - Atomicity: A transaction happens fully or not at all.
 - Consistency: Data stays valid before and after the transaction.
 - Isolation: Transactions don’t affect each other, even if they run at the same time.
 -  Durability: Once saved, data stays safe even after a system crash.
These systems power live business apps, like banking or retail systems. Often referred to as line of business (LOB) applications.

### Analytical data processing
<img width="1188" height="270" alt="image" src="https://github.com/user-attachments/assets/a827303e-87f5-4dd9-a90b-3276c35a8bd0" />
<img width="594" height="135" alt="analytical-processing" src="https://github.com/user-attachments/assets/f83047a3-72b0-4c25-8558-6d037a103227" />

