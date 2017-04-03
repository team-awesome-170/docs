
# Introduction


1.1 Purpose
-----------

This document's purpose is to incorporate and collect all concrete &
abstract ideas of the Fast Cards systems first release, Release Number
1.0. This Software Requirement Specification will provide granular
details as well as overarching epics to all parties involved. Parties
including but not limited to; Team-Awesome Developers, current Project
Manager Dale Fletter, Product Owner CSUS Computer Science Department,
and future users (CS Instructors, or other) of the Fast Cards system.

1.2 Document conventions
------------------------

Documents sections should be developed with headings numbered
sequentially. Sub-sections should have sub-headings and numbered
sequentially in the form x.1, x.2. For any lists bullets points should
be used over numbers unless there is a specific need to reference
individual list entries.

1.3 Project scope
-----------------

The Faculty Information Card System will a webpage for user to input the
faculty information

and an interface with other database to automatically update daily; and
design the specific Fast

Cards for user the printing out. Other requirements are exclusive in the
project. A detail

specification is available in the project vision and scope document that
submitted in Sprint 1.

1.4 References
--------------

California State University Sacramento Space Management

http://www.csus.edu/aba/space/

# Overall Description


2.1 The Product Perspective
---------------------------

Product Need: Every semester the computer science must generate the
faculty information cards individually without any centralized
management.\
Product Scope: Currently the product is only for the computer science
department but could potentially be expanded to serve other academic
departments.

**Product definition**:

A tool that retrieves information about a faculty member from a database
system and uses that information to generate faculty information cards.
The request can be automated and integrated into a website or requested
by a user and printed for faculty members to display.

**Major Features:**

User interface (CRUD) -The interface and the operations that the users
use to interact with the system.

DSS(Data Storage System)- The database the will hold all the information
entered by the users. The database storage system should consist of a
database, a database management system and an operating system running a
web server.

2.2 User Classes and Characteristics
-------------------------------------

### Classifying users

**System Admin:** This user class manages all components of the system
including the database and operating system for the application
environment.

**Application Admin:** This user class only administers the application
and the data contained within. Can execute all CRUD operations

**Application User:** This user class only can execute read and update
operations.

### Stakeholder Profiles

**CS Department** - Currently this is Veronica Pruitt: Office
Administrator, and Andrew: Clerk.

**Instructor(s)** - The Professors and Lecturers in the CS department.

**System Admin** - ECS computing services

2.3 Operating Environment
--------------------------

Fast Cards will run and be served from an Apache web application server
which includes a MySQL database that can be installed on the same server
or a remote system. The server(s) will be/may be located anywhere but
access and administration will be performed by campus IT personnel and
must be accessible from computers located on campus.

The Fast Card application server will also need to be capable of sending
and accepting emails to request and receive the office hours for
teaching faculty.

Users of Fast Cards can access the system using the following supported
browsers and versions:

-   Internet Explorer ver. 9+

-   Mozilla Firefox ver. 45.8+

-   Google Chrome ver. 57+

-   Apple Safari 10+

2.4 Design and Implementation Constraints
-----------------------------------------

Space Management will inform the Computer Science department regarding
the the space availability.

Then the Computer Science(CS) department members (Reyna Yvette and
Veronica Pruitt) will update the database with a csv file. The CS
faculty will have access to a user interface(UI) that will help them
update the database. The UI will be running in a server that makes an
API call to the Database and stores the necessary information.

Instructors will also have access to a UI that will make API calls to
the get the necessary information, but they will not be able to update
the any csv files. Instructors will just get the card information and
print it out themselves.

2.5 Assumptions and Dependencies
--------------------------------

-   All users of the Fast Card software have access to a computer with internet access to connect to the application.

-   Users are assumed to have been provided a valid email address with which their account will be associated with in order to access the software.

-   The software is dependent on the classroom assignments which are provided by the space management department. The assignments are delivered to the CS dept. in CSV format.

-   Computer Science Department will have access to printing and perform other postproduction requirements (i.e. cutting/separating cards from Avery card stock) with sufficient capabilities to handle the volume of cards produced by the system.

Appendix A
----------

### Definitions

**UI** - User Interface: the space where the user interacts with the
machine and the applications

**CRUD** - Create Read Update Delete

**Faculty Information Cards** - Printed Cards display the most recent
information about faculty member contact info and office hours.

**DSS** - Data Storage System: the database and database management
system that is planned for the app.

**ABA** - Administration and Business Affairs: find more information at
[*http://www.csus.edu/aba/about.html*](http://www.csus.edu/aba/about.html)

**Space Management**: a department with the ABA that determines the
classroom assignments every semester.

**CSV** - Comma Separated Value: A file that stores tabular data in
plain-text format.
