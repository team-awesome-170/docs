#1. Business Requirements

##1.1 Background
The CS department must post Faculty Information Cards each semester outside the office where they sit.  The information cards are printed for each semester to include information for the faculty member, the courses he/she teaches, and office infomration including location, phone number and times that the faculty member can be found there.

Classroom schedule data is pulled from Space Management which reports to ABA and loaded into a local database.  Faculty then emails their office hours which are entered manually into the database.  Once all of the information for the cards has been entered into the local database, A mail merge is performed with a Word template to prepare the Faculty Information Cards for printing.

##1.2 Business Opportunity
A new software system should be designed and implemented that will ease the administrative burden required to produce the printed Faculty Information Cards.  The system needs to be usable by staff without requiring a high degree of technical skills.  The software should be generalized so that it may be easily migrated or scaled to other departments, campuses or schools.

The software is intended for internal department.  Optionally, other departments may utilize the system but will be required to have their own administrator and clerk.  Any administrator would be able to set up their own clerk, create another department and grant authority to the admin or reset another admin's password.

The new system can streamline some of the administrative overhead by allowing faculty to access the system and enter their own office hours as well as automate the ETL process when downloading the schedule data from Space Management.

##1.3 Business Objectives
##1.4 Success Metrics
##1.5 Vision Statement
##1.6 Business Risks
##1.7 Business Assumptions and Dependencies

#2. Scope and Limitations
##2.1 Major Features
##2.2 Scope of Initial Release
##2.3 Scope of Subsequent Releases
##2.4 Limitations and Exclusions

#3. Business Context
##3.1 Stakeholder Profiles
__Office Administrator__ (Veronica Pruitt) - Downloads class schedule data from Space Management (ABA) and transfers to local database (ETL).  Receives office hour information by email and enters this information into the database.

__Clerk__ (Andrew ? ) - Pulls data from local database and uses Microsoft Word mail merge to prepare the Faculty Information Cards for printing.

__CS Department Faculty__ - Notifies Veronica Pruitt by email of office hours.

__Students__ - Relies on faculty information cards to get meet with faculty for help outside of class.

__IT Staff__ - There may or may not be IT staff required to install faculty information card software, setup/maintain database and maintain respective servers.

##3.2 Project Priorities
##3.3 Deployment Considerations
