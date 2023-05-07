# E-commerce Back End Starter Code

E-commerce also known as internet retail, is the largest sector of the electronics industry,Different e-commerce platforms provide a suite of services to businesses of all sizes.Due to the prevalence of these platforms, developers should understand the fundamental architecture of e-commerce sites.

So this application is the back end for e-commerce site.In this I used working Express.js API and configure it to use Sequelize to interact with a MySQL database.This application won't be deployed.So user have to test this application in insomnia.Also for this application I clone startercode as per challenge requirement and then I pushed this clone in my github repository. In this ecommerece-back-end application, user can see 3 tables like Category, product and Tag.and in backend user can see all data, specific one data, create data, update particular data, and delete data for all three tables.also all tables is related with each other.so main this is one backend application in which user can create CRUD operation on table data.

Here I explained how this ecommerce-back-end application have to create and work,

- First in Develop folder, user can see different folders.
- In assests folder, I saved application screenshots and gif and video files.
- In config folder, Connection.js file is used to create connection with database using sequenlize and with dotenv file.dotenv file genereally used for to do privacy reason to protect database,username and password.
- In db folder, schema.sql file shows which databse and table use in this application.
- In models folders,index.js file shows relation between tables like foreignKey and association between tables belongsto,hasmany,belongsMany,belongstoMany.and in Category.js, Product.js,ProductTag.js,Tag.js create table using sequelize and constraints on columns like primary key, not null, unqiue,auto increament etc.
- In routes folder, index.js files shows main route like '/api' and in api folder, index.js files shows different routes for categories,products and tags js files. categories.js file shows GET, GET by particular id, POST, PUT, DELETE sequelize query so user can run CRUD opertion in insomnia for categories. as same operations done in proucts-routes.js file for products and taag-routes.js file for tags.
- In seeds, it shows as particular data in particular table like in category-seeds.js shows category data, product-seeds.js shows product data,tag-seeds.js shows tag data.etc
- In .env files shows database name,user name and password.
- server.js file shows how to use express and routes in this applicaiton. server.js is main file.

In this application, I used express, sequelize,mysql2, dotenv insomnia, so I improved my knowledge in this topics. also from this application I learned how can we create tables in sequelize and perform CRUD opertion in data using sequelize also how to test this queries in insomnia.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)

# Installation

In this application, I used express, sequelize, mysql2. so here are some steps user have to perform before start the application.

- first, right click on "db folder", and click open integreted terminal, run mysql -u root -p, if user have password enter password. and then run source schema.sql, quit. so user can initize database and table .

- on server.js right click , select open in imtegreted terminal, run npm install so all dependencies which are using this application saved. or user have to install all dependencies like

  - npm install express
  - npm install dotenv
  - npm install mysql2
  - npm install sequelize

- in package.json file, "scripts" have "seed" in which its run node seeds/index.js file and "start" its run node server.js file. so user can enter commands like

  - npm run seed
  - npm run start or node server.js

- so application starts execution, user have to check all of this queries in insomnia. I show all queries outputs in assests folder.also in usage option as under.

# Usage

Here I attached some .gif of insomnia.

![DB_Application_run_get_all](./Develop/assests/DB_application_run%20_insomnia_GET.gif)
![GET_ALL](./Develop/assests/GET_ALL.gif)
![Categories](./Develop/assests/GET_POST_PUT_DELETE_Categories.gif)
![Products](./Develop/assests/GET_POST_PUT_DELETE_Product.gif)
![Tags](./Develop/assests/GET_POST_PUT_DELETE_Tag.gif)

A walkthrough video demonstrating the functionality of the application and all of the acceptance criteria being met.- https://drive.google.com/file/d/1Ll3tb2vfBKlJ8mDFc92AMM8HuF3gvgvF/view

The URL of the GitHub repository. -
https://github.com/avanijadeja/ecommerce-back-end

# Credits

for this application, I read from diffrent websites as mention below.

    1. https://www.w3schools.com

    2. https://dev.mysql.com/doc/

    3. https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise

    4. https://sequelize.org/

    5. https://expressjs.com/

# License

This project is using the MIT License.

# Badges

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
