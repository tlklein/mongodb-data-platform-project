# MongoDB Exercises
This folder contains a series of exercises designed to help users practice basic MongoDB operations such as creating databases, inserting documents, querying collections, and using advanced query operators. The exercises include screenshots and explanations to guide users through each task.

## Exercise A: Create and List Databases
1. Create a new database named `employees` using the `use` command.
2. List all databases on your MongoDB instance.
![Exercise A](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-a.png)


## Exercise B: Create, Drop, and List Collections
1. Create a database named `temporary`, add a collection named `test` to it, and then drop the database. Report the output of `show dbs` and `show collections` before and after the database drop.
![Exercise B1](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-b.png)

2. Create multiple collections using department names in the database created in Exercise A.
3. List all collections in the current database.
![Exercise B2](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-b2.png)


## Exercise C: Inserting and Retrieving Documents
1. Insert some employee documents with fields (employee id, name, and salary) into multiple collections created in previous exercises.
2. Use the `find` command to retrieve all the entered data.

![Exercise C](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-c.png)

## Exercise D: Querying Documents
1. Add the following employees to any collections.
2. Find 2 documents using the `employee id` field.
3. Find all documents where the `name` field starts with "John".
4. Find all documents where the `name` field contains "John".
5. Find 2 documents using the `name` field.

![Exercise D](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-d.png)


## Exercise E: Working with `zips.json`
0. Import the `zips.json` file into MongoDB.

![Exercise E0](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-import.png)

1. Get all cities with a population of less than 1500.
![Exercise E1](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-e1.png)

2. Find all data for the city "CHESTER" using a query operator.
![Exercise E2](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-e2.5.png)

3. Use the array query operator to find all entries for locations at `(-84.38570799999999, 45.015207)`.
![Exercise E3](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-e2.png)

4. Use a logical operator to find all entries that match the city "WARREN", or the location at `(-80.76424299999999, 41.231819)`.
![Exercise E4](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-e3.png)


## Exercise F: Using the `$where` Operator
1. Use the `$where` operator to find all employees with a salary over 75,000.
2. Use the `$where` operator to find all employees where the `name` contains "John".
![Exercise F](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-f.png)


## Exercise G: Querying Specific Fields
1. Using only one collection from the `employees` database, query all documents in that collection but return only the `name` and `salary` fields.
![Exercise G](/Vue.js%20Projects/MongoDB%20Queries/screenshots/hm2-part-g.png)
