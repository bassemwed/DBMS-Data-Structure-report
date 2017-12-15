# DBMS-Data-Structure-report


Welcome to the DBMS-Data-Structure-report Copied from article

IT Article -- DBMS & Data Structure

Ms. Nidhi Goyal SYMCA [07MCA16]

Better Database design by Data Structure concepts/Relationship between Database and Data Structure Concepts

In today’s era every person is directly or indirectly connected with the concepts of data structures and database and they consider both of these concepts as different. But the reality is that, database and data structure have some relationship between them.

No doubt database is a collection of data which can be stored, updated, data can be retrieved any time when required. But when it comes to store data in database many decision about, how data will be stored? How efficiently data can be retrieved from database? How efficiently the data in database can be modified and many such questions arise.

One of the solutions for such a problem is using the concepts of data structures that can involve the way data will be stored, easy and efficient retrieval, etc.

Data Structure refers to the actual implementation of the data type and offers a way of storing data in an efficient manner. Data Structure is an outcome of application of certain tools and techniques used to connect data items within records and between records of the same file or of different files. A proper selection and design of data structure helps users to access and manipulate the records of files in a database in an efficient manner. The main objective of a data structure is to organize data to suit a specific purpose so that data can be accessed and worked both efficiently and effectively. Data Structure may be designed to store data for the purpose of working on it by using different algorithms for searching or sorting data. Algorithms are the essential aspect of data structures and as there are many algorithms for searching and sorting, they differ in terms of efficiency. When efficiency is involved, it would be nice to have metrics for comparing algorithm efficiency.

The complexity of algorithm depends upon two perspectives:

Time Complexity: It is a function describing the amount of time an algorithm takes in terms of the amount of input to the algorithm.
Memory/Space Complexity: It is a function describing the amount of memory an algorithm takes in terms of the amount of input to the algorithm.

When data is to be accessed from the database there are generally three different ways:

The basic mission of a database management system is to, upon request, return part of the database to the requester. In a relational database, what’s returned will be a record or set of records whereas in an object-oriented database it will be an object or set of objects; and so on.
In a few major brands of data warehouse appliance, the DBMS may call pretty much the whole database into memory, then find what it wants from there. Most other DBMS are more finicky, and try to retrieve from disk only the data requested.
More precisely, they usually retrieve data blocks of a fixed size, and try to bring back only the blocks that may contain the information being looked for.

At the core, most data access methods are consisting of two things:

Data Structure
A design for indexes that point into that data structure.

There are many kinds of data structure, with some of the most important being:

Arrays with fixed-length entries:

There’s nothing faster than getting data from a completely regular array. Only thing to be done is to calculate the address and whole of the array can be accessed. But again, lack of compression is a huge issue. One of the examples of this data structure is SAS Intelligence Storage.

Tables with variable-length entries:

One of the most important data structures of modern database management is the table, storing numeric, date or character-string data.

Linked list (hierarchy or network):

In this data structure a pointer would accompany each data value to the next one you were likely to want. Here link is from a parent, children and next-records. These systems were called hierarchical if there only was one parent (e.g., IBM’s).

Stack Data Structure:

It is a data structure used to maintain the records of a file where there is no need to maintain any order among the records of the file. In this structure, the records will be added as well as deleted at the top end of the stack. The principle followed in retrieving records from the stack is Last-In-First-Out (LIFO).

Inverted List Data Structure:

The records of a file may be retrieved based on different keys on different occasions. This can be possible by creating an index file for each and every key field or secondary key field of main file. The index values in the index file will help to locate the records of the main file quickly which in turn reduces the overall response time of the query.

Index:

A database index is the most widely used data structure that improves the speed of operations on a database table. They can be created using one or more columns of a database table, as a basis for rapid random lookups and efficient access of ordered records. One of the advantages of using index is that it requires less disk space to be stored. The other great benefit of indexes is that the server doesn’t have to work as hard to get the data as they are much same as book indexes, providing the database with quick jump points to find the database row. But at the same time if too many indexes can slow the database down. So indexes speed up finding data, but slow down inserting, updating or deleting data. There are many more data structures that can be used in different situations according to need. As discussed earlier not only the storage structure is to be maintained but also the data types in terms of their range are to be considered while designing a database. After all the space occupied in memory is also a crucial point to be discussed. As the program for managing the database changes the data types with their range also changes. Thus the range of a data type is also an important issue. When designing a database, one should really try to understand the data, and the data type that suits it best. If we take example of CHAR. It supports fixed width strings, up to 8,000 characters and is best used when data length is constant, whereas VARCHAR supports variable length strings, up to 8,000 characters (2000 bytes) and is best used when data length is variable. Because CHAR is a fixed-length data type, the storage size of the CHAR value is equal to the maximum size for this column. Because VARCHAR is a variable-length data type, the storage size of the VARCHAR value is the actual length of the data entered, not the maximum size for this column. One can use CHAR when the data entries in a column are expected to be the same size and VARCHAR can be used when the data entries in a column are expected to vary considerably in size. Apart from CHAR and VARCHAR, VARCHAR2 can also be used that supports 4000 bytes of data, which is best, used when one requires to add any further updatation (i.e. increase the size of data) which is not possible with the case of VARCHAR. The most important difference is that CHAR is padded with spaces and VARCHAR is not. For example, if you have:

CREATE TABLE temp (t1 VARCHAR (2), t2 CHAR (2));

INSERT INTO temp (t1, t2) VALUES ('a', 'a'); The column t1 will contain value 'a', while column t2 will contain value 'a ' with additional space.
