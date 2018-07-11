# ClassRoomOptimizationSys
SCOPE OF PROJECT
The scope of this project will provide direction and help one stay on target with regards to the areas covered by this project and in the other hand suggests additional work that might likely be done on the application in the future.
This project has two major aspect, the ADMIN and USER side. The Admin using the automatic functions provided by the system to assign Lecture DAY, TIME and VENUE of best capacity to courses to form a standard school timetable. The User on the other hand has access to the system only to view the timetable which has been scheduled by the admin. 
Note that the Admin only gives instruction to the system who goes ahead to assign Day, Time and Best Venue to courses automatically.
The case study used in this project is University Of Nigeria Nsukka, Computer Science department.

Below are the detailed duties of the Admin and the User.
USERS
•	Views school timetable that has been automatically provided by the system on the instruction of the admin.
When the users visit the site, they will be welcomed by an awesome page called “SplashScreen.aspx” and then the application will open for them to have direct access to school timetable. They don’t need to login for it is only the admin that needs to go through that process. (When the application opens, the page that contains the timetable that the Users see is called “TimeTableUsers.aspx”)
The users can only View the Timetable whose venues, time and day of lecture are already assigned by the system. (N:B It is only the admin that has the permission to perform this operation of assigning venue, day and time to courses. Also note that what the admin actually does is to just click a button to instruct the System to automatically assign the best venue, day and date to a course that is selected “not that he does it manually by himself”. He gives this instruction to the system by just clicking “Assign Venue” link and the system will do all the necessary checks and assign the best lecture venue, time and day to the course)
If the admin has not instructed the system to assign venue, day and time to any Course, The Users can only see a blank page with an empty timetable.
ADMIN					
•	Instructs the System to assign day, time and venue of best capacity to courses to form a standard timetable which will be made available to users by the system.
When the Admin logs into the system, he will see a Timetable comprising of both the courses whose lecture venues, day and time have already been assigned (or allocated) to them and those ones without venue, day and time yet. His Timetable is different from what the users sees when they visit the site. Users are accessing “TimeTableUsers.aspx” page which contains a finished standard timetable whose venue, day and time of lecture has already been assigned by the admin whereas the Admin is accessing “TimeTableAdmin.aspx” page which has additional controls which enables the Admin to instruct the system to automatically assign venue, day, and time to courses to form a standard timetable.
 Those Items in the timetable he will see that doesn’t have Venue, day of lecture and time yet are waiting for him (ie the admin) to instruct the system to automatically assign the best aforementioned elements to them.
The Items on the admin Timetable with “Status” True already have lecture Venues, time and day assigned to them.
Whereas those Items on the admin Timetable with “Status” False have not been assigned Lecture Venue.
To assign Lecture venues to those items without venues yet, the admin will click on the “Assign Venue” Links on the side of each item on his timetable. (Example:: MON | COS 462 | 10 – 12 | with 200 as the number of students that registered the course. “let’s assume he selected this record”)
When he clicks on the above timetable record, (ie when he clicks the Assign Venue link), the system will pick the ID of the record he selected and
Check If there is a lecture venue whose capacity is equal to the no of students that registered the course he selected on the timetable (ie 200 from the example we are handling). If it sees a venue like that, it will sign that venue to that course.
If it didn’t see, it will automatically check if there is a venue whose size is immediately above 200, say 205. If it sees, it will assign that venue to that course
But if it didn’t see, it will automatically check if there is a venue whose size/capacity is just immediately 200 say 195. If it sees, it will assign it to the course. 
It automatically assigns Day and Time of the lecture to the selected course.
When the admin clicks Login Button, it takes him to a page called “Login.aspx” where he provides his login credentials to access the system.
When he logs out, it returns him to a general User environment where he can only view the system as an ordinary user.



