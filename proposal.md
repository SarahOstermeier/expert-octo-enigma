# X-Team 84 Dorm Room Assignment Project Proposal

## Goal
To provide an efficient program and interface for assigning students to dorm rooms.

## Problem Description

Assigning dorms and rooms to incoming students, and matching students with a compatible roommate (assuming 2 roommates per dorm room).

To achieve this, our program creates a class for the students and a class for the dorms. Student preferences are stored within the student class and dorm information is stored in the dorm class, including room numbers and locations. Also an algorithm that can match roommates.

For testing the student class, we will formulate JUnit tests for each input type (preferences, interests, etc.). Included in these tests will be tests for each method that ensures user information can be changed and is changed correctly. We will also have tests that make sure all fields have been filled in to ensure no null values(User should select no choice if they do not have an opinion).
For testing the room class, we will use JUnit to create tests that ensures no duplicate names per room, tests to make sure that input data is stored correctly and can be compared to a student object. Tests to ensure an error message is returned if a null student is inputted. Tests to make sure only 2 memebers can be stored and if more are added an exception roomFullException should be thrown. Tests to ensure that members can be replaced or removed from a room.
For testing, we would create JUnit tests to test if we can, for exmaple, properly generate Student classes, properly store large numbers of Students, properly see if a Room is available or not, etc.


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



