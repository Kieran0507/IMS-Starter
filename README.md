Coverage: 70.9%
# Project Title

One Paragraph of project description goes here

## Getting Started

To get started you will need to run the sql-data.sql schema to initiate your database and then using command line navigate to where you stored the Jar file and launch it using "java -jar ims-0.0.1-jar-with-dependencies" 

### Prerequisites

To use this software you will need a system running java and MySQL

MySQL can be downloaded here
https://dev.mysql.com/downloads/windows/installer/8.0.html

An installation guide can be found here
https://dev.mysql.com/doc/mysql-installation-excerpt/5.7/en/



### Installing

To get a dev enviroment you will need a java IDE to open the project in and JDK

JDK:
https://www.oracle.com/java/technologies/downloads/


You will now need to import the project into your chosen ide

File > Open projects from file system > navigate to where you saved the project > select the IMS-Starter folder


You should now be able to view and launch the project in a dev enviroment


Now lets launch the application using either command line or in your chosen ide

you can now type to match the available options to navigate the system
lets try creating a customer
1. type customer to select this entity
2. type create
3. entire the desired information as prompted
4. well done you created your first entry

Now lets view that customer
1.select customer if not already selected
2.select read
3. you should now be viewing your saved customers

Warning: you cannot add customers or items to an order if they don't exist in the system yet



## Running the tests

To run the tests right click the project in your chosen IDE and then

run as > JUnit test 
or
coverage as > JUnit test

### Unit Tests 

Each individual testable method has been tested you can run these as above

example:
@Test
	public void testCreate() {
		final Customer created = new Customer(2L, "chris", "perrins");
		assertEquals(created, DAO.create(created));
	}

this test will try to create a customer and add them to the database, it will then check this was achieved correctly



## Deployment
Any problems or help needed with deployment or other issues please contact me on K.goodinson94@gmail.com for live support 

## Built With

* [Maven](https://maven.apache.org/) - Dependency Management



## Authors

* **Chris Perrins** - *Initial work* - [christophperrins](https://github.com/christophperrins)
* **Kieran Goodinson** - *rest of the work* - [Kieran0507](https://github.com/Kieran0507)

## License

This project is licensed under the MIT license - see the [LICENSE.md](LICENSE.md) file for details 

*For help in [Choosing a license](https://choosealicense.com/)*

## Acknowledgments

* Jordan Benbelaid & Reece Elder - for helping me learn java
* Reece Taylor - Prompting me on how to get around problems i was confused with
* Google - answering lots of questions
* QA - for helping me take a step into coding
