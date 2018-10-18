# X-Team 84 Dorm Room Assignment Project Proposal

See https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code for tips on using *Markdown* tags to format __.md__ files

## Goal

Work as a team to create a project proposal for your X-team to complete together.
The project does not have to be extremely difficult,
but there must be work to do for each member of your team.
You may reference figures using "See figure 1".  
Be sure to submit corresponding image files, i.e. figure1.png (or figure1.jpg) for each figure.

## Grading: To earn full credit, your team's proposal must include:

* (md) documentation: [this file] describing purpose and use of your program

* Description of a program that has:

  ** a main Java program class in a file named Main.java
  
  ** a custom data structure designed and built by your team
  
  ** comprehensive testing of individual units
  
 Caution: You are not being asked to implement this program, at least not yet. 
 We just want your group to make a proposal or pitch for your program.
 
 Tip: Your custom data structure can be composed of or extensions of data structures that you have learned and used in previous programming assignments.  We're looking for decisions about how to build a high-level data structure that will likely have lower-level components.

## Problem Description

Assigning dorms and rooms to incoming students, and matching students with a compatible roommate (assuming 2 roommates per dorm room).

To achieve this, our program creates a class for the students and a class for the dorms. Student preferences are stored within the student class and dorm information is stored in the dorm class, including room numbers and locations. Also an algorithm that can match roommates.

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



## Edit and Submit this file and any figures referenced by this document.

