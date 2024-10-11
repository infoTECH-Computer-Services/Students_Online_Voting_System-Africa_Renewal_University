# Students Online Voting System - Africa Renewal University
KAYE Voting System is a cutting-edge, web-based solution designed to transform student elections at Africa Renewal University (AfRU) by integrating blockchain technology to eliminate voter intimidation and enhance election security, transparency, and accessibility.

Africa Renewal University (AfRU) currently conducts its student elections using a traditional paper ballot system. This process has inherent challenges, including voter intimidation, lengthy voting processes, and the potential for manual errors. Voter intimidation has been a particularly significant problem, discouraging students from participating in elections.
The need for a more secure, transparent, and efficient election process led to the proposal of a web-based voting system using blockchain technology. This system aims to prevent voter intimidation by allowing students to cast their votes online from any location while maintaining security, transparency, and efficiency.

#	PROBLEM STATEMENT
Voter intimidation at AfRU undermines the democratic process by creating an environment of fear, coercion, and misinformation that can create a hostile environment that deters individuals from freely expressing their voting choices. Voter intimidation, which involves actions like aggressive questioning, physical blocking of polling places, using threatening language, disseminating false information, or disrupting voting lines, is illegal and can lead to severe penalties in the context of university elections, where students exercise their right to vote.

In a world free from voter intimidation, students would feel safe exercising their voting rights, confident that their votes would be counted accurately without any external influence. The blockchain-based voting system aims to create an environment, that reduces voter intimidation and ensures transparency, security, and efficiency in the voting process.

This study seeks to design and implement a web-based student voting system using Blockchain Technology related to its transparency, security, integrity, efficiency, and reliable electoral process to reduce voter intimidation and foster a fair and transparent election process at AfRU by which any student can use his/her voting rights from anywhere in the country to transmit votes over the phones, private computers, or the Internet, without the need to visit a polling booth on campus in person.

# OBJECTIVES OF THE PROJECT STUDY
##	Main objectives: 
The main objective of this study is to design and implement a secure, efficient, fast, accurate, user-friendly interactive Web-based student voting system using Blockchain Technology to prevent voter intimidation in the AfRU student elections.

##	Specific objectives:
1.	To study how voter intimidation affects the current manual voting process at AFRU.
2.	To design a blockchain-based voting system that enhances transparency, security, and a systematic way of conducting voter registration and candidate applications.
3.	To develop and implement the designed web-based voting system that properly manages the voters’ rights in the election in a well-organized manner.
4.	To test the designed system to ensure it successfully prevents voter intimidation and maintains election integrity.

#	JUSTIFICATION OF THE PROJECT STUDY
##	To science
This study will contribute to the growing body of knowledge on blockchain-based voting systems, particularly in educational institutions. It will provide insights into how blockchain can be used to improve election security and transparency, and it may serve as a reference for future researchers in similar domains.
##	To Society
By implementing this blockchain-based voting system, AfRU will benefit from a more secure, transparent, and efficient election process. The system will eliminate voter intimidation and encourage more students to participate in elections, leading to a more representative student council.

#	DESIGN METHODOLOGY CHOICE 
In this study, a combination of Object-Oriented Design (OOD) and Data-Flow Oriented Design (DFD) methodologies was used to design the system, ensuring that both the flow of data and the relationships between system components are mapped out.
##	Object-Oriented Design (OOD)
OOD is used to structure the system into objects (voter, admin, ballot, etc.) that interact with one another. This methodology ensures the system is modular, scalable, and easy to maintain. Key design components include:
- **Use Case Diagrams:** These represent the various interactions between the system and its users (e.g., how a student logs in and votes).
-	**Class Diagrams:** These represent the structure of the system, identifying key classes (e.g., Voter, Ballot, Admin) and their relationships.

##	Data Flow-Oriented Design (DFD)
DFD is used to map the flow of data between the different components of the voting system. It helps in understanding how data (votes, voter details) flows from one point to another, ensuring that there are no bottlenecks or security gaps in the system. Key diagrams include:
1.	Context-Level DFD (Level 0): This represents the entire system, showing how votes flow from voters to the blockchain, and how results are processed.
-	**External Entities:** Voter, Admin, Blockchain Network
-	**Process:** KAYE Online Voting System
-	**Data Stores:** Voter Database (MySQL), Vote Data Store (Blockchain)

2.	High-Level DFD (Level 1): This shows the major processes within the voting system.
-	**Voter Registration:** Inputs: Voter submits registration details (Name, Registration Number, Email). Process: Voter data is validated and stored in the Voter Database. Outputs: Confirmation email sent to the voter.
-	**Vote Casting:** Inputs: Voter logs in and selects candidates. Process: Voter credentials are authenticated. A vote is securely cast and stored on the Blockchain. Outputs: Confirmation email sent to the voter.
-	**Vote Tallying:** Inputs: Admin requests election results. Process: Votes are tallied from the blockchain. Outputs: Results are displayed on the admin dashboard and voters can view the final election outcome.

#	Database Design
The Database Design of the KAYE Online Voting System ensures the secure storage of voter information, candidate details, and voting records. The database is structured around key entities such as Voter, Admin, Candidate, Vote, and Position. Relationships between these entities ensure data integrity and support the voting process.

The database consists of the following key tables:
-	**User Table:** Contains voter details, such as ID, registration number, first name, last name, email, password, photo, and date created.
-	**Votes Table:** Records the votes cast by each voter, linking them to candidates and positions.
-	**Candidates Table:** Stores information about the candidates running for different positions.
-	**Admin Table:** Contains information about the administrators managing the election process.
-	**Positions Table:** Stores the names and IDs of the positions available in the election.


#	System Flowchart
The System Flowchart for the KAYE Online Voting System provides a visual representation of the steps involved in the voting process, from voter authentication to vote submission and tallying. This diagram outlines the logical flow of actions taken by both the voters and the system, helping to ensure that all critical operations are executed in sequence.

The flowchart includes the following key steps:
1.	**Voter Login:** Voters authenticate themselves using their registration number and password.
2.	**Voter Authentication:** The system checks the validity of the credentials.
-	If valid, the voter proceeds to the next step.
-	If invalid, an error message is displayed, and the voter is asked to retry.
3.	**Vote Casting:** The voter selects candidates for the available positions.
4.	**Vote Submission:** The voter submits the ballot, and the system stores the vote securely on the blockchain.
5.	**Confirmation:** After submission, the voter receives a confirmation message and email.
6.	**Vote Tallying:** Admins access the tallying process, where votes are counted, and results are displayed.
The following figure illustrates the overall flow of the KAYE Online Voting System, detailing the sequence of operations for voters and admins.

#	Programming Languages
The development of the blockchain-based voting system relies on various programming languages and frameworks for both the front end and back end. These tools ensure that the system is secure, responsive, and user-friendly.

##	Frontend Technologies
### 1.	HTML (HyperText Markup Language):
-	**Purpose:** HTML is the standard markup language used to structure content on the web. It is used to create the skeleton of the web-based voting interface, defining the structure of web pages, including elements such as forms for voter registration, voting buttons, and candidate lists.
-	**Role in the Project:** HTML is used to create the voting system’s user interface (UI), ensuring that it is visually structured and accessible to all voters.

### 2.	JavaScript:
-	**Purpose:** JavaScript is a versatile programming language used to add interactivity to web pages. It handles the dynamic behaviors of the voting system, allowing the system to respond to user inputs, validate voter forms, and communicate with the backend (e.g., submitting votes).
-	**Role in the Project:** JavaScript manages frontend operations such as form validation (e.g., checking that all required voter information is entered correctly) and sending data to the server or blockchain using Ajax.

### 3.	AJAX (Asynchronous JavaScript and XML):
-	**Purpose:** AJAX allows web pages to communicate with the backend asynchronously without needing to reload the entire page. This is essential for creating a smooth user experience.
-	**Role in the Project:** In the voting system, AJAX is used for real-time communication between the front end and the back end. For example, it enables live updates on the voting progress, such as dynamically displaying confirmation messages after a vote is cast, without refreshing the page.

### 4.	jQuery:
-	**Purpose:** jQuery is a fast, small JavaScript library that simplifies tasks such as HTML manipulation, event handling, and AJAX calls.
-	**Role in the Project:** jQuery is used to simplify JavaScript code for frontend tasks. For instance, it provides an easier way to handle form submissions, AJAX calls, and animations on the voting interface.

### 5.	Bootstrap:
-	**Purpose:** Bootstrap is a popular CSS framework that provides pre-designed templates for responsive web design. It ensures that the web-based voting system is visually appealing and works well on various devices, including desktops, tablets, and smartphones.
-	**Role in the Project:** Bootstrap is used to create a responsive voting interface. This ensures that the system is user-friendly across different screen sizes, providing a consistent experience for voters on both mobile devices and desktops.

##	Backend and Database
### 1.	PHP (Hypertext Pre-processor):
-	**Purpose:** PHP is a server-side scripting language commonly used for backend development in web applications. It handles server-side logic, database connections, and API calls.
-	**Role in the Project:** PHP is used to handle backend operations such as voter registration, authentication, and database interactions with MySQL. When a voter registers or logs in, PHP scripts verify credentials and ensure the right data is fetched from the database.

### 2.	MySQL (Relational Database):
-	**Purpose:** MySQL is a widely used open-source relational database management system. It stores structured data and allows for easy querying and retrieval.
-	**Role in the Project:** MySQL is used to store non-voting-related data such as voter registration details (name, email, student ID) and candidate information. While votes themselves are stored on the blockchain for security, voter data is stored in MySQL, allowing the system to easily authenticate voters and ensure that only eligible users participate in the election.

### 3.	Solidity:
-	**Purpose:** Solidity is a high-level programming language used to write smart contracts on Ethereum’s blockchain. It allows for decentralized applications to run securely on the Ethereum platform.
-	**Role in the Project:** Solidity is used to create smart contracts that automate the voting process, ensuring security and transparency. The smart contracts handle critical tasks like vote casting, vote tallying, and enforcing election rules. For example, once a vote is cast, the Solidity smart contract automatically encrypts and stores the vote on the Ethereum blockchain, making it immutable and tamper-proof.
-	**Blockchain Role:** Solidity is the core language used to interact with the Ethereum blockchain, ensuring that all transactions, including votes, are securely recorded and that results are transparently auditable.
