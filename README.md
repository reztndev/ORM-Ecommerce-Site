# Module 13: (Object Relation Mapping): E-commerce Website

## Summary
In this challenge, we'll build an E-commerce website that utilizes the latest backend technologies to support its commercial operations, including:
1. Postgres database for storing and managing the products that the commerce site offers
2. Sequalize, a Node.js Object Relational Mapper (ORM) tool, that is used to configure and interact with the Postgres database
3. Express.js for implementing and serving the various routes (APIs) that may be used to perform the standard CRUD (Create, Read, Update, Delete) operations of the database models which include:
* Categories of products
* Products 
* Tags which are specific attributes that may be attached and associated with a given product

## Application Setup
To provide a headstart in creating and running the commerce site, sample seed data is provided to populate the database models for Category, Product, Tag and ProductTag.  To accomplish the seeding, the following database needs to be created via Postgres's shell:
* ecommerce_db

A schema.sql is provided for facilitating this task.

Once the database is created, the corresponding and aforementioned models need to be seeded by running the following in the command shell:
* npm run seed

You'll notice that the seeding scripts are included in the corresponding seed definition files for each model in the database. Also notice that the database relationships between the models, such belongsTo, hasMany & belongsToMany, are defined in the index.js under the project's models folder

## Operation
Once the database is created and models are seeded, the application may be started by running the following in the command shell:
* npm start

This command will start up the server which makes it possible to issue the various CRUD operations on the aforementioned database items, such as the following examples:
1. GET localhost:3001/api/products (which fetches all products)
2. GET localhost:3001/api/products/:id (which fetches an existing product identified by its id)
3. POST localhost:3001/api/product (which creates a new product)
4. PUT localhost:3001/api/product/:id (which updates an existing product identified by its id)
5. DELETE localhost:3001/api/product/:id (which deletes an existing product identified by its id)

As mentioned, the CRUD operations may be issued against all models that are stored in the database and are not limited to the example above which illustrates such operations being performed on the model Product.

To create or update an item, you'll need to study the corresponding model definition files under the project's model folder, or by studying the model's seed definition files under the seed folder.

## Exercising the Routes
You will need to install, set up and use an API development and testing tool such as Insomnia.

## Recorded Video of the Site's Operation 
A recorded video of the site's functioning, which specifically illustrates the invocation of CRUD operations, is available via the following link: https://app.screencastify.com/v2/manage/videos/H8B2nMizCXwyUDekNj3y
