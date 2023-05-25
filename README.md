# Taxi Service
Mini taxi service simulation project. The user has the ability to create a driver, car and manufacturers, add a manufacturer to a car, and add a driver to cars. It is possible to view all cars, manufacturers, drivers and cars available to the current driver

# Features

* Authentication
* Display all drivers
* Display all cars
* Display cars for current user
* Display all manufactures
* Create new driver(which is user)
* Create new car
* Create new manufacturer
* Add driver to car

# Project structure

* Controller
  * car
    * AddCarController - create new car
    * AddDriverToCarController - add driver to car
    * DeleteCarController - delete car
    * GetAllCarsController - get all car
    * GetMyCurrentCarsController - get current user cars
  * driver
    * AddDriverController - add drive
    * DeleteDriverController - delete driver
    * GetAllDriversController - get all driver
  * manufacturer
    * AddManufacturerController - add manufacturer
    * DeleteManufacturerController - delete manufacturer
    * GetAllManufacturerController - get all manufacturer
  * IndexController - start page
  * LoginController - authentication 
  * LogoutController - logout
* dao
  * CarDaoImpl - CRUD operation with car
  * DriverDaoImpl - CRUD operation with
  * ManufacturerDaoImpl - CRUD operation with manufacturer
* exception - custom exception for CRUD
* lib - Injector and annotation 
* model
  * Car model
  * Driver model
  * Manufacturer model
* Service (handling all business logic)
  * AuthenticationServiceImpl - 
  * CarServiceImpl
  * DriveServiceImpl
  * ManufacturerServiceImpl
* Util
  * ConnectionUtil - instance of connection to DB
* web.filter
  * AuthenticationFilter - web filter to redirect unauthenticated user to login page
* resources script for SQL 
* webapp jsp pages and web.xml configuration file

#  Used technologies and libraries

* Java 11
* Apache Maven 4.0
* Apache TomCat 9.0.74
* Git
* JDBC 
* MySql
* JSP 
* JSTL 1.2
* JavaxServlet 4.0.1

# For launching the project

    1 Clone this repository
    2 Install SQL and run script init_db.sql
    4 Update ConnectionUtil with parameters of your SQL server 
    4 Configure Apache TomCat 9
    5 Run TomCat server and use web application