
# 1. Business Requirements

## 1.1 Background

The CS department must post Faculty Information Cards each semester outside the office where they sit.  The information cards are printed for each semester to include information for the faculty member, the courses he/she teaches, and office infomration including location, phone number and times that the faculty member can be found there.

__Questions__

* How is the information to complete the cards currently stored (database, spreadsheet, etc..)  
* How are the cards completed and printed (word template?)


## 1.2 Business Opportunity

A new software system should be designed and implemented that will ease the administrative burden required to produce the printed Faculty Information Cards.  The system needs to be usable by staff without requiring a high degree of technical skills.  The software should be generalized so that it may be easily migrated or scaled to other departments, campuses or schools.

The software is intended for internal department.  Optionally, other departments may utilize the system but will be required to have their own administrator and clerk.  Any administrator would be able to set up their own clerk, create another department and grant authority to the admin or reset another admin's password.


## 1.3 Business Objectives
    *Shah*
	To create a software service that automatically updates the required Faculty information into printed information card. 
## 1.4 Success Metrics
    *Shah*
Acceptance criteria 1: The system should includes the automation of the necessary information being printed into all the cards using information provided by the user.
Acceptance criteria 2: The system should also be capable of printing a single card upon request.
Acceptance criteria 3: The information about a faculty member should only be changeable by the office administrator.
Acceptance criteria 4: The entry of faculty office hours and the viewing of all information is allowed for the clerk.
 
Bonus acceptance criterias:
	a. System would allow the generation of new semester based on the information from the prior semester and keep both in the database. 
        b. System would allow the system to print cards for departments other than just the CS department.
        c. Each department has its own administrator and clerk
        d. Only an administrator can setup a clerk
        e. Each administrator can setup an academic department and grant authorities
        f. No administrator should be able to see the data of a different department.

## 1.5 Vision Statement
    *Shah*
To create a user-friendly automated software that helps CS faculty administration generate accurate Faculty information cards.
## 1.6 Business Risks
      a.  No business risks have been identified.
      
## 1.7 Business Assumptions and Dependencies
      a. It is assumed the the department will have an office administrator who will approve changes made to faculty member information. The system therefore is dependent on having an application administrator.
      b. The department must have a printer in order to print the faculty office hour cards.
      c. It is assumed that the department has the necessary technology infrastructure to host a database and the administrators necessary to support the environment this application will run within.  
      d. The application administrator or clerk depend on faculty members to submit changes to their information.
      e. The application administrator or clerk depend on information about the assignment of classrooms.    

# 2. Scope and Limitations

## 2.1 Major Features

## 2.2 Scope of Initial Release

## 2.3 Scope of Subsequent Releases

##  2.4 Limitations and Exclusions
      a. The option to create multiple academic is not planned for this release but will be an additional feature in future releases. 

# 3. Business Context

## 3.1 Stakeholder Profiles

__CS Department Faculty__

__Office Administrator__

* changes information about a faculty member (exclusive privilege) 

__Clerk__

* able to change information about office hours but not faculty information

__Students__

__Questions__

* Would a DBA be required to setup/maintain the database and would database or other IT staff be considered a stakeholder?


## 3.2 Project Priorities

## 3.3 Deployment Considerations

