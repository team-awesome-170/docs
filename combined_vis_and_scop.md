# California State University, Computer Science Department
## Faculty Information Cards: Vision and Scope Document


Version 1.0

Prepared by: Aitken, Connor | Binjola, Devesh | Duan, Cindy | Hairabedian, Bryce | Newaz, Shah | Wadsworth, Robert

CSC170 Section 01 -- Fletter, Dale

February 22, 2017

#1. Business Requirements
##1.1 Background
The Computer Science (CS) department must post faculty information cards each semester outside the office where they sit.  The information cards are printed for each semester to include information for the faculty member, the courses he/she teaches, and office infomration including location, phone number and times that the faculty member can be found there.

Classroom schedule data is pulled from Space Management (SM) which reports to Administration & Business Affairs (ABA) and loaded into a local database.  Faculty then emails their office hours which are entered manually into the database.  Once all of the information for the cards has been entered into the local database, A mail merge is performed with a Word template to prepare the Faculty Information Cards for printing.

##1.2 Business Opportunity
A new software system should be designed and implemented that will ease the administrative burden required to produce the printed Faculty Information Cards.  The system needs to be usable by staff without requiring a high degree of technical skills.  The software should be generalized so that it may be easily migrated or scaled to other departments, campuses or schools.

The software is intended for internal department.  Optionally, other departments may utilize the system but will be required to have their own administrator and clerk.  Any administrator would be able to set up their own clerk, create another department and grant authority to the admin or reset another admin's password.

The new system can streamline some of the administrative overhead by allowing faculty to access the system and enter their own office hours as well as automate the ETL process when downloading the schedule data from Space Management.

##1.3 Business Objectives
The business objective is to create an automated tool where it takes the required information fr
om a database system and use that information to generate faculty information cards.

##1.4 Success Metrics
*Acceptance criteria 1*: The system should includes the automation of the necessary information being printed into all the cards using information provided by the user.
   
*Acceptance criteria 2*: The system should also be capable of printing a single card upon request.
    
*Acceptance criteria 3*: The information about a faculty member should only be changeable by the office administrator. 

*Acceptance criteria 4*: The entry of faculty office hours and the viewing of all information is allowed for the clerk.
        
__Bonus acceptance criterias__  
a. System would allow the generation of new semester based on the information from the prior semester and keep both in the database.  
b. System would allow the system to print cards for departments other than just the CS department.  
c. Each department has its own administrator and clerk  
d. Only an administrator can setup a clerk  
e. Each administrator can setup an academic department and grant authorities  
f. No administrator should be able to see the data of a different department

##1.5 Vision Statement
To create a user-friendly automated software that helps CS faculty administration generate accurate faculty information cards.

*Desired End-State*: A sleek software tool that helps the CSUS faculty administration create information cards.

##1.6 Business Risks
a. No business risks have been identified for the implementation of this system. If the system is adopted, having a single admin is a potential single point of failure. The system should consist of a global administrator(s), application administrator(s), and user(s) for a more robust management framework. 

##1.7 Business Assumptions and Dependencies
a. It is assumed the the department will have an office administrator who will approve changes made to faculty member information. The system therefore is dependent on having an application administrator.  
b. The department must have a printer in order to print the faculty office hour cards.  
c. It is assumed that the department has the necessary technology infrastructure to host a database and the administrators necessary to support the environment this application will run within.  
d. The application administrator or clerk depend on faculty members to submit changes to their information.  
e. The application administrator or clerk depend on information about the assignment of classrooms.    

#2. Scope and Limitations
##2.1 Major Features
Elevator Pitch: A partially automated Faculty card system for the Department of Computer Science
 California State University Sacramento.

Capable of housing all pertaining information relating to the Faculty Card per each faculty member, updating or creation of new faculty/class information, and the actul printing of the faculty card after such information has been verified by all parties.

Parties, Users include Computer Science Department (currently Veronica Pruitt & Andrew), Instructor, ABA(Administration & Business Affairs), and Admin to the system.
    
##2.2 Scope of Initial Release
### Users
* Computer Science Department
* Instructor
* System Admin
    
### Initial Release
The initial release will consist of a large subset of desired features. These features are provided in terms of User Story epics that convey the scope of work to be considered "Done."

* As a __*Computer Science Department*__ I need to be able to Print the Faculty Cards so that I can deliver current, correct, and up-to-date schedules for students and colleges to see.
* As an __*Instructor*__ I need to be able to Update my Faculty Card information so that I can provide students with up-to-date information.
* As a __*System Admin*__ I need to be able to alter how the system works so that the Faculty Card system can adapt to change or resolve any issues that may arise.

##2.3 Scope of Subsequent Releases
### Deliverables to be diferred in initial release
* Option to provide multiple rooms per Course-Section
* Custom Stylizing of Card per Instructor
* System Metrics and Measurements per Faculty Card
* Option to include email under "Office Phone" for more contact options
* Print from desk option for Instructor

##2.4 Limitations and Exclusions
a. The option to create multiple academic is not planned for this release but will be an additional feature in future releases.

#3. Business Context
##3.1 Stakeholder Profiles
__Office Administrator__ (Reyna) - Downloads class schedule data from Space Management (ABA) and transfers to local database (ETL).  Receives office hour information by email and enters this information into the database.

__Clerk__ (Alysia) - Pulls data from local database and uses Microsoft Word mail merge to prepare the Faculty Information Cards for printing.

__Computer Science Department Faculty__ - Notifies Veronica Pruitt by email of office hours.

__Students__ - Relies on faculty information cards to get meet with faculty for help outside of class.

__IT Staff__ - There may or may not be IT staff required to install faculty information card software, setup/maintain database and maintain respective servers.

##3.2 Project Priorities
* Features: all features scheduled for release 1.0 must be fully completed, and matches all the functional requirements. 
* Quality: Have to pass 97% of user acceptance tests, (including: login, security, functions, and system performance tests). 
* Schedule: Phrase1 of project are scheduled to be available on 20 May, 2017. Overrun of up to 2 weeks acceptable without sponsor approval. 
* Cost: +15% budgets difference are acceptable without sponsor review. Project manager is responsible for communicating and review the expenses with financial department of cost business unit. 
* Staff: total team size is six team members: 2 developers, half-time tester, 1 project manager will have 50% of time for project management, half-time for Business Analyst. Additional 1 member can be borrowed from other team if necessary during the project period. Team members will be encouraged to wrap up a strong, high quality program in order to leave enough time to carefully plan a well-structured, and prepare for system go-live, and problem solving.
* Change Management: any requirements changes request by customer, project manager is responsible to communicate with related teams, and set up meeting to address it.  Any adjusts cost up to 40 man hours. Project manager has to submit additional resource request, and signature by project manager of client. Project manager is responsible to communicate with market department if there is any cost outside of contract.

##3.3 Deployment Considerations
The Oracle database 12.12 is required to be installed on the database server, and apple browser and windows explore need to be upgraded to the newest version on the web server. Application server have to be ready one day before promote all the program objects from test environment to production. One additional backup printer has to be ready for print the faculty information cards. 
