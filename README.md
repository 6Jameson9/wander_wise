# Report on Creating an SQLite Database and Implementing CRUD Operations in a Flutter Application
## WanderWise SQLite Database Implementation

### Introduction
This report outlines the implementation of an SQLite database and CRUD (Create, Read, Update, Delete) operations within a Flutter application. The application in question, WanderWise, incorporates user authentication and profile management features. We utilized the sqflite package for database interactions and provided a seamless user experience across different platforms by using sqflite_common_ffi for non-web platforms and sqflite_web for web.

### Project Setup
To begin, we set up the necessary dependencies in `pubspec.yaml`:

```yaml
dependencies:
  flutter:
    sdk: flutter
  sqflite:
  sqflite_common_ffi:
  path:
  flutter/services.dart:
  flutter/material.dart:
```
# Database Initialization
## We created a DatabaseHelper class to handle database interactions. This class initializes the database and defines the schema for the users table.

Database Schema
The users table schema includes the following fields:

usrId: INTEGER PRIMARY KEY AUTOINCREMENT
fullName: TEXT
email: TEXT
usrName: TEXT UNIQUE
usrPassword: TEXT
