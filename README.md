## Project Title
    Mobile Application for Transacation.

## Getting Started
    These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

## Prerequisites
    What things you need to install the software and how to install them.

    Node.js
    Flutter
    PostgreSQL
    Installing

## Clone the repository.

    git clone https://github.com/yourusername/yourproject.git

## Install dependencies.

    cd node-server
    npm install

## Set up the PostgreSQL database.
    Connect to database by using this command
    plsql -U posgress  and then enter the password      you will enter password at the instalation of DB postgres so don't forget it 
    
    Create a database named app.
    CREATE DATABASE your_database_name;
    Connect to the database 
    \c your_database_name
    Create a table named users with columns id (serial primary key), email (text), and password (text).
    CREATE TABLE users (
        id SERIAL PRIMARY KEY,
        username VARCHAR(50) UNIQUE NOT NULL,
        password VARCHAR(50) NOT NULL
    );

## Start the backend server.

    node server.js

    don't forget to configure conenction of database 
    
    const pool = new Pool({
      user: 'postgres',
      host: 'localhost',
      database: 'app',
      password: 'atrox123', 
      port: 5432,
    }); 
## Run the Flutter app.
    cd flutter_app
    flutter run -d browser 

Built With
Flutter - Frontend framework
Node.js - Backend server
PostgreSQL - Database
Authors
Amine Rhayem && khaled ihit 
