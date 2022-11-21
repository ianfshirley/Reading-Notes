## MongoDB and Mongoose

### SQL vs NoSQL

Fill in the chart below with five differences between SQL and NoSQL databases:

| SQL | NoSQL |
|:---:|:---:|
| relational based database | non-relational/distributed database |
| table based DB | document based DB / key:value pairs / graph DB / wide-column stores |
| predefined schema | dynamic schema for unstructured data |
| vertically scalable | horizontally scalable |
| uses Structured Query Language | queries are focused on collection of documents (unstructured query language) |

1. What kind of data is a good fit for an SQL database?
- data with complex queries
2. Give a real world example.
- Oracle
3. What kind of data is a good fit a NoSQL database?
-  hierarchical data storage
4. Give a real world example.
-  MongoDB
5. Which type of database is best for hierarchical data storage?
-  NoSQL
6. Which type of database is best for scalability?
-  They are both scalable, but it seems like horizontal scaling/adding new servers with NoSQL seems more efficient.

### Video: SQL vs NoSQL

1. What does SQL stand for?
- Stuctured Query Language
2. What is a relational database?
- Not really explained in the video, he just says it means that it works with SQL. I think it means that the data is structured as a table, and the header row of the table will hold certain 'keys'. Each subsequent row is another data item, and each column in that row will be a 'value' that corresponds to the table header of that column. There can also be related tables, one table getting data from multiple other tables, or 1:1 tables.
3. What type of structure does a relational database work with?
- table data
4. What is a ‘schema’?
- it's basically the table header. it means that each item in the table needs to fit the schema (must have a value for each key)
5. What is a NoSQL database?
- MongoDB
6. How does it work?
- It has collections instead of tables. Inside of those collections there are documents. These documents are similar to the rows in the SQL tables, but they don't need to fit the same schema. 
7. What is inside of a MongoDB database?
- collections of documents
8. Which is more flexible - SQL or MongoDB? and why.
- MongoDB - no schema
9. What is the disadvantage of a NoSQL database?
- there will be some duplicate data, the same thing might have to be updated in multiple different places, vs. updating it in one place in SQL will update it everywhere because it's relational.

### Sources

[SQL vs NoSQL](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)<br>
[Video: SQL vs NoSQL](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)<br>
[Mongoose API](https://mongoosejs.com/docs/api.html#Model)<br>
[React Router](https://v5.reactrouter.com/web/api/BrowserRouter)<br>