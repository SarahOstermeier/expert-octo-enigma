# X-Team 84 Dorm Room Assignment Project Proposal

## Goal
To provide an efficient program and interface for assigning students to dorm rooms.

## Problem Description

Assigning dorms and rooms to incoming students, and matching students with a compatible roommate (assuming 2 roommates per dorm room).

To achieve this, our program creates a class for the students and a class for the dorms. Student preferences are stored within the student class and dorm information is stored in the dorm class, including room numbers and locations. Also an algorithm that can match roommates.

For testing the student class, we will formulate JUnit tests for each input type (preferences, interests, etc.). Included in these tests will be tests for each method that ensures user information can be changed and is changed correctly. We will also have tests that make sure all fields have been filled in to ensure no null values(User should select no choice if they do not have an opinion) if a null value is inserted then an exception fieldsNotFilledException().

For testing the room class, we will use JUnit to create tests that ensures no duplicate names per room, tests to make sure that input data is stored correctly and can be compared to a student object. Tests to ensure an error message is returned if a null student is inputted. Tests to make sure only 2 memebers can be stored and if more are added an exception roomFullException() should be thrown. Tests to ensure that members can be replaced or removed from a room.

For testing the Main class, we will have tests that form an event that our event listeners should catch and checks to make sure something happens. Tests that contain 1 student with the same preference and a few locations with only 1 that meets the preferences. Tests to make sure if all students have the same preference then students are inserted in first come first serve order. Tests that contain many students and many dorms that the assign method should properly handle. Tests for correct exceptions being thrown when there is no student/room/dorm data. NoInputException(). Tests to make sure the event listener for inputting a student changes the interface to the student interface and that this event listener correctly handles fieldsNotFilledException().

For testing the dorm class, we will test the setIncomingStudents by passing students to see if it works. Also we will pass null students and students exceed the capacity of the dorm to see if it throw exceptions correctly. For number of rooms, we will test if negetive number is rejected. For the assignroommate method, we will test if this method give each student a room number, fill each room with 2 students. Moreover, we would test if the assignment follow the students preference by setting a correct answer and see if the program's result is the same as us. We would test the corner cases and the exception like assigning roomates when there is no enough space, or no enough students.

## Questions to answer for Exercise #2

1. Name: Dorm Room Assignment



2. Output: A room assignment with 2 students attached.

Format: DORM, ROOM#, [Student1], [Student2]

Example: Dejope, 311, Sarah Ostermeier, Diana Li




3. Input: List of dorms and rooms, list of students and roommate preferences

List of dorms and rooms:

Format: [DormName], [#ofRooms]

Example: Dejope, 200

List of studnets and roommate preferences: 

Format: [studentName],[Preference]

Example: Yan, Jason




4. User Interface: 
[See figure 1](https://github.com/SarahOstermeier/expert-octo-enigma/blob/master/main%20interface.png)
[See figure 2](https://github.com/SarahOstermeier/expert-octo-enigma/blob/master/student%20interface.png)




5. Types List: 

Main class: Will contain an event listener that will respond to the user clicking a button on the interface. When a button is clicked on the main interface, the event listener will respond by calling the appropriate methods. For example, when the user clicks "Register Student", the event listerner will call a constructer in the student class and construct a new student. 


Student class: Store information about each students.

fields: String StudentName, String Roommate preference, Dorm preference.

Methods: getName(); getPreference();


Room class: Store information about each room in the dorm

fields: Student Roommate1, student Roommate2;

Methods: String getRoommates(); void setRoommate(Student students); boolean isAvaliable();


Dorm class: store all the rooms in the dorm

fiels: Room[] rooms, Student[] student

Method: setIncomingStudnet(Studnet newStudnet), setNumberOfRooms(int rooms), void assignRoommate().



