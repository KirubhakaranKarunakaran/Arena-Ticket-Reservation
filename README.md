# Arena-Ticket-Reservation
Homework Assignment
	
ARENA TICKET
RESERVATION

Homework Assignment
Application Manual

Submitted by
Kirubhakaran Karunakaran
8-Oct-2015

 
1. INTRODUCTION 
1.1 PROJECT OVERVIEW
The Arena Ticket Reservation system is an implementation of simple ticket service that facilitates the discovery, temporary hold, and final reservation of seats within a high-demand performance venue. This Application helps the customers to search the availability and prices of various levels of arena and allows the user to hold or reserve the seats. This project also covers various features like reserving the already held seats, checking the reservation.
2. PRODUCT DESCRIPTION
2.1 PRODUCT PERSPECTIVE
The Arena Ticket Reservation system is written in JAVA language using MAVEN tool and is completely independent. The application would be running on a Windows Operating system
2.2 PRODUCT FEATURES
The Arena Ticket Reservation system has the following features
The system is only intended for customers or end-users. The features of this system can be categorized four main categories.
a.	Check Seat Availability
b.	Hold the preferred seats
c.	Reserve seats
d.	Check the reserved seats

Home Page:
Arena Ticket Reservation homepage presents the options of Checking seat availability, Making Reservation, Reserving the Held seats, Checking your reserved seats and to quit the application. The homepage requests the user to provide an option (from the above) to proceed with the function.
Check Seat Availability:
Check Seat Availability option finds the number of seats available within the arena in the level which is of interest to the user. This function requests the user to provide the level id of arena (according to the below table) in which he is looking for seats. The function validates the level selected by the user. Once validated, based on the level selected, the application gets the available seats information back to the user. (If the seat is held by some other user, that won’t be counted available).
 
Hold the Preferred Seats:
Hold Preferred Seats option looks for the best available seats with in the specified levels of user interest and holds the seats for the user. This function requests the customer Email, number of seats, preferred minimum and maximum levels of interest. The function validates these information and requests user to input the values again if the information provided is not valid. Once validated the function checks if the requested seats are available according to the user’s preference. If available, the function returns the seats information along with level name, price of each ticket and the total amount for this reservation to the user. The function also requests for the user’s option to go ahead and reserve the selected seats, to hold the selected seats and go back to main menu or to quit the application. If the user chooses to reserve the seats straightaway it invokes the Reservation function. If the user chooses to hold the seats and to go back to main menu, the seats will be held for a minute and the user will be provided with a seat hold id and will be taken back to home page. If the user selects to quit, it will exit the application.
Reserve Seats:
Reserve Seats option is called in two scenarios. 
a)	Reserve the best seats selected from the option2 of the homepage.
In this scenario, when the user chooses to go ahead with the reservation after finding the best seats available, the seats will be reserved for that user and he will be provided with a confirmation code.

b)	Reserve the already held seats from the option3 of the homepage.
In this scenario, the application requests the customer email from the user and validates it. If valid, the function checks for the available seats that are in hold for the provided email. If a valid hold exists for this email, the seats will be booked for the user and will be provided with a confirmation code. If no valid hold exists with that email, the user will be provided with the message saying that there is no valid hold exists.
Check the reserved seats:
Check the reserved seats function requests the customer email from the user. The application checks if a valid reservation exists for this email provided. If exists, the user will be provided with the seat reservation details. The details include Level name, Number of seats, Total price and Confirmation code. If no reservation exists for the provided email, the user will be provided with a message saying no reservation exists for the provided email.
2.4 User Characteristics:
There is only one kind of user for the Arena Seat Reservation system and it is the customer.

2.5 Compiling and Test instructions:
Download the HomeWork folder from GITHub to your local drive.
Important Note: Please make sure the user has write/modify access to the folder.
 
Open the command window for the HomeWork folder.
Compile command line:  mvn clean compile
This will compile the code and create class files. You will get the message, saying BUILD SUCCESS.

Package creation and tests command line: mvn clean package
This will create a jar file for the application and run the tests provided in the folder.
The jar can be located under target folder.
 
Execution:
To execute, go to the folder HomeWork\target\classes
Application Execution command line: java com.reservation.ticket.MainClass
 
The application gets executed and provides the user with the Welcome page
 
