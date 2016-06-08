## Domain Analysis and Software Design(X556-1)Project

### Title : Project Helper Application

### Team Name : Kimkidol

### Team Member : 
+ 201220936 KimKiwoo
+ 201220961 KimKihong
+ 201420990 JeongEunseon
+ 201420995 ParkSungmi
+ 201421020 SonMinseok


### Develop environment
1. android : Windows 8 K, android studio, Java
2. server : Linux, MySQL 5.0.95, PHP


### Files
1. pha.zip
  + zip file which has android studio project

2. server.zip
  + zip file which has codes in project's server. Folders in this file must be in the server.
  + If you want to use your own server, let these folders are in server's /www folder and need to change host address in android code and mysql information in server code

3. app-debug.apk
  + apk file for the project


### Compile and Run
+ This project is android application, so you need to build it in Android Studio. 
+ Import this project with Android Studio (The android project's name is pha)
+ To build the project, you should click Build | Make Project
+ To run the project, you should click Run | Run 'app' and then choose the device.


### Function

#### Authentication page
 - There are two blanks and two buttons : ID, password / sign in, sign up
 - Users put their ID and password in the blanks and sign in.
 - If they donot have their own account, they can sign up with sign up button.
 - It requires userID, password, studentID, Name for sign up.

#### Initial page
 - There are two tabs on top of the screen.
 - First tab is for user's timetable, and the other team list.

#### Timetable tab
 - User's private timetable is taken most part of the screen and there is a button on the bottom.
 
##### Timetable
 - Each block of the timetable means 30minutes.
 - TImetable display lectures from 9AM to 9PM.
 - gray-colored-block means empty and orange-colored block with text means there is a lecture at the time.
 
##### Button
 - Once user click the button, two other buttons come up.
 - First button is for adding lecture and the other for deleting.
 - Adding lecture requires lectureName, lectureRoom, professorName, and lectureTime. Except lectureTime, all data is inserted by user with keyboard. User need to choose lectureTime on the screen.
 - Deleting lecture requires lectureName that user want to do.

#### Team list tab
 - All team lists that user is joined are shown on the white part of the screen and there is a button on the bottom.
 
##### Team list
 - Team list contain teamName, and lectureID.
 - User can click one of team list when he/she wants to enter the team page.

##### Button
 - There are a button on the bottom for add team.
 - adding team requires teamName and lectureID.

#### Team page
 - User can see a teamTimetable and a button.
 
##### Team timetable
 - team timetable gives information about all members' lectures to users.
 - There are three block types. white means empty, and orange the team schedule leader made. Combining all members' timetables, for each block, it become black if at least one member has a lecture at the time.

##### Button
 - Once leader click the button, three buttons come up, but member can see only second and third buttons.
 - First button is for adding member and it requires member's ID.
 - Second button is for adding team schedule and it requires scheduleName, place, and time.
 - Third button is for deleting team schedule and it requires time.


