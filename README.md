# SRS-of-ATM
 detail study of ATM software. 
        by #AmitPethkar
Software Requirement Specification 
ATM 
 
					
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
     			-By Amit Pethkar
 
Page 18 
 
 
 
Table of Contents 
 
1. Introduction  
 
1.1 Purpose  
 
1.2 Scope  
 
1.3 Definitions, Acronyms, and Abbreviations  
 
1.4 References  
 
1.5 Overview  
 
2. The Overall Description  
 
2.1 Product Perspective  
 
2.2 Product Functions  
 
2.3 User Characteristics  
 
2.4 Constraints  
 
2.5 Assumptions and Dependencies  
 
3. External interface Requirements  
 
3.1 User Interfaces  
 
3.2 Hardware Interfaces  
 
3.3 Software Interfaces  
 
3.4  Communications Interfaces  
 
4. System Features  5. Other Non-Functional Requirements  
5.1 Performance Requirements  
5.1.1 Capacity  
5.1.2 Dynamic Requirements  
5.1.3 Quality  
 
5.2 Software System Attributes  
3.6.1 Reliability  
3.6.2 Availability  
3.6.3 Security  
3.6.4 Maintainability  
5.3 Business Rules  
 
 
6. Other Requirements.............................................................................  
 
Appendix A: Glossary 
 
Page 19 
 
 
1. Introduction 
 
The software ATM version1.0 is to be developed for Automated Teller Machines (ATM). An automated teller machine (ATM) is computerized telecommunications device that provides a financial institution's customers a secure method of performing financial transactions, in a public space without the need for a human bank teller. Through ATM, customers interact with a user-friendly interface that enables them to access their bank accounts and perform various transactions. 
 
 
1.1 Purpose 
 
This SRS defines External Interface, Performance and Software System Attributes requirements of ATM version1.0. This document is intended for the following group of people:- 
 
 
 Developers for the purpose of maintenance and new releases of the software. 
 
 Management of the bank. 
 
 Documentation writers. 
 
 Testers. 
 
 
 
1.2 Scope 
 
This document applies to Automated Teller Machine software ATM version1.0. This software facilitates the user to perform various transactions in his account without going to bank. This software offers benefits such cash withdrawals, balance transfers, deposits, inquiries, credit card advances and other banking related operations for customers. It also allows the administrator to fix the tariffs and rules as and when required. 
 
The software takes as input the login Id and the bank account number of the user for login purposes. The outputs then comprise of an interactive display that lets the user select the desirable function that he wants to perform. 
 
The software is expected to complete in duration of six months and the estimated cost is Rs. 10 lakhs. 
 
 
1.3 Definitions, Acronyms, and Abbreviations. 
 
 
 
AC 	Alternate Current 
AIMS 	ATM Information Management System. 
ATM 
 
 	An unattended electronic machine in a public place, connected to a data system and related equipment and activated by a bank customer to obtain cash withdrawals and other banking services.
Braille 
 
 	A system of writing and printing for blind or visually impaired people,  in  which   varied  arrangements  of   raised  dots representing letters and numerals are identified by touch. 
BMS 	Bank Management Software developed by KPM Bank. 
 
Page 20 
CDMA 	Code Division Multiple Access, a reliable data communication protocol. 
CMS 	Card Management Software developed by KPM Bank. 
DES 	Data Encryption Standard. 
Dial-Up POS 	A message format for low cost communications. 
Electronic Journals 	For easier, safer information storage, related to modem. 
 
Internet 
 	An   interconnected   system   of   networks   that   connects computers around the world via the TCP/IP protocol. 
MB 	Mega Bytes 
ms 	Milliseconds. 
sec 	Seconds 
Smart Card 
 	Card without hardware which stores the user’s private keys within a tamper proof software guard. 
SRS 	Software Requirements Specification. 
Tactile keyboard 	Special keyboard designed to aid the visually impaired. 
 
TCP/IP 	Transmission Control Protocol/Internet Protocol. 
V 	Volts 
VGA 	Video Graphics Adaptor is a display standard. 
 
 
1.4 References 
 
The references for the above software are as follows:- 
 
i.	www.google.co.in  
 
ii.	www.wikipedia.com  
 
iii.	IEEE. Software Requirements Specification Std. 830-1993.  
 
iv.	Chevy Chase Bank, UMBC Branch.  
 
v.	Russell C. Bjork Requirements Statement for Example ATM System. Online.  
URL: http://www.maths-cs.gordon.edu/local/courses/cs211/ATMExample/ 
 
 
 
 
 
 	 
 
Page 21 
 
 
 
 
1.5 Overview 
 
Section 1.0 discusses the purpose and scope of the software. 
Section 2.0 describes the overall functionalities and constraints of the software and user characteristics. 
Section 3.0 details all the requirements needed to design the software. 
 
2. The Overall Description 
 
2.1 Product Perspective  
 
 
 
 The ATM is a single functional unit consisting of various subcomponents. 
 
 This software allows the user to access their bank accounts remotely through an ATM without any aid of human bank teller. 
 
 This software also allows to perform various other functions apart from just accessing his bank account such as mobile bill clearings etc. 
 
 Some of its hardware components are cassettes, memory, drives, dispensers i.e. for receipts and cash, a card reader, printer, switches, a console, a telephone dialer port, a networking port and disks. 
 
 The ATM communicates with the bank’s central server through a dial-up communication link. 
 
 The Memory of the system shall be 20MB. 
 
 The Cassette capacity shall be at least 2000 notes. 
2.2 Product Functions  
 
The major functions that ATM  performs are described as follows:- 
 
 
 Language Selection:- After the user has logged in, the display provides him with a list of languages from which he can select any one in order to interact with the machine throughout that session. After the language selection the user is prompted with an option that whether he wants the selected language to be fixed for future use so that he is not offered with the language selection menu in future thus making the transaction a bit faster. User also has the freedom to switch to a different language mentioned in the list in between that session. 
 
 Account Maintenance:- The various functions that a user can perform with his account are as follows:- 
 
 Account Type:-The user has the freedom to select his account type to which all the transactions are made, i.e. he can select whether the account is current account or savings account etc. 
 
 
 	 
 
 
 
 
 
 Withdrawal/Deposit: The software allows the user to select the kind of operation to be performed i.e. whether he wants to withdraw or deposit the money. 
 
 Amount:- The amount to be withdrawn or deposited is then mentioned by the user. 
 
 Denominations:- The user is also provided with the facility to mention the required denominations. Once he enters his requirements the machine goes through its calculations on the basis of current resources to check whether it is possible or not. If yes, the amount is given to the user otherwise other possible alternatives are displayed. 
 
 Money Deposition:- Money deposition shall be done with an envelope. After typing the amount to be deposited and verification of the same, the customer must insert the envelope in the depositary. 
 
 Balance Transfer:- Balance transfer shall be facilitated between any two accounts linked to the card for example saving and checking account. 
 
 Balance Enquiry:- Balance enquiry for any account linked to the card shall be facilitated. 
 
 Billing:- Any transaction shall be recorded in the form of a receipt and the same would be dispensed to the customer. The billing procedures are handled by the billing module that enable user to choose whether he wants the printed statement of the transaction or just the updation in his account. 
 
 Cancelling:- The customer shall abort a transaction with the press of a 
Cancel key. For example on entering a wrong depositing amount. In addition the user can also cancel the entire session by pressing the abort key and can start a fresh session all over again. 
 
 Map locating other machines:- The machine also has a facility of displaying the map that marks the locations of other ATM machines of the same bank in the entire city. 
 
 Mobile Bills Clearings:- The machine also allows the user to clear off his pending mobile bills there only, if the name of his operator is mentioned there in the list. The machine displays the list of the companies supported by that bank to the user. 
 
Department of CSE, 
SDBCT, Indore Page 
23 
Software Engineering 
& Project 
Management Lab 
Manual 
 
 
 
 
2.3 User Characteristics 
 
There are different kinds of users that will be interacting with the system. The intended users of the software are as follows:- 
 
 
 User A: A novice ATM customer. This user has little or no experience with electronic means of account management and is not a frequent user of the product. User A will find the product easy to use due to simple explanatory screens for each ATM function. He is also assisted by an interactive teaching mechanism at every step of the transaction, both with the help of visual and audio help sessions. 
 
 User B: An experienced customer. This user has used an ATM on several occasions before and does most of his account management through the ATM. There is only a little help session that too at the beginning of the session thus making the transaction procedure more faster. 
 
 Maintenance Personnel: A bank employee. This user is familiar with the functioning of the ATM. This user is in charge of storing cash into the ATM vault and repairing the ATM in case of malfunction. This user is presented with a different display when he logs in with the administrator’s password and is provided with options different from that of normal user. He has the authority to change or restrict various features provided by the software in situations of repairing. 
2.4 Constraints  
 
The major constraints that the project has are as follows:- 
 
 The ATM must service at most one person at a time. 
 
 The number of invalid pin entries attempted must not exceed three. After three unsuccessful login attempts, the card is seized/blocked and need to be unlocked by the bank. 
 
 The simultaneous access to an account through both, the ATM and the bank is not supported. 
 
 The minimum amount of money a user can withdraw is Rs 100/- and the maximum amount of money a user can withdraw in a session is 
 
 
Department of CSE, SDBCT, Indore 
Software Engineering & Project Management Lab Manual 
 
 
 
Rs.10,000/- and the maximum amount he can withdraw in a day is Rs 
20,000/- 
 
 
 Before the transaction is carried out, a check is performed by the machine to ensure that a minimum amount of Rs 1000/- is left in the user’s account after the withdrawal failing which the withdrawal is denied. 
 
 The minimum amount a user can deposit is Rs 100/- and the maximum amount he can deposit is Rs 10,000/-. 
 
 A user can select only that cellular operator for mobile bill clearings that is supported by the bank. 
 
 The software requires a minimum memory of 20GB  The database used should be Oracle7.0. 
 
 There shall be a printer installed with the machine to provide the user with the printed statement of the transaction. 
 
 For voice interactions, speakers should also be there to accompany the machine. 
2.5 Assumptions and Dependencies  
 
 
 
The requirements stated in the SRS could be affected by the following factors: 
 
  One major dependency that the project might face is the changes that need to be incorporated with the changes in the bank policies regarding different services. As the policies changes the system needs to be updated with the same immediately. A delay in doing the same will result to tremendous loss to the bank. So this should be changed as and when required by the developer. 
  Another constraint relating to the operating environment is that we are specific to Oracle Database. 
  The project could be largely affected if some amount is withdrawn from the user’s account from the bank at the same time when someone is accessing that account through the ATM machine. Such a condition shall be taken care of. 
  At this stage no quantitative measures are imposed on the software in terms of speed and memory although it is implied that all functions will be optimized with respect to speed and memory. 
 
 
 
It is furthermore assumed that the scope of the package will increase considerably in the future. 
 
 
3. External Interface Requirements 
 
Department of CSE, SDBCT, Indore 
Software Engineering & Project Management Lab Manual 
 
 
3.1.1 User Interface Requirements  
 
The interface provided to the user should be a very user-friendly one and it should provide an optional interactive help for each of the service listed. The interface provided is a menu driven one and the following screens will be provided:- 
 
1.	A login screen is provided in the beginning for entering the required  username/pin no. and account number.  
2.	An unsuccessful login leads to a reattempt (maximum three) screen for again entering the same information. The successful login leads to a screen displaying a list of supported languages from which a user can 
	 	select any one.  
3.	In case of administrator, a screen will be shown having options to reboot  	system, shut down system, block system, disable any service.  
4.	In case of reboot/ shut down, a screen is displayed to confirm the user’s  will to reboot and also allow the user to take any backup if needed.  
5.	In case of blocking system, a screen is provided asking for the card no. 
By entering the card no of a particular user, system access can be  blocked for him.  
6.	Administrator is also provided with a screen that enables him to block any service provided to the user by entering the name of the service or 
	 	by selecting it from the list displayed.  
7.	After the login, a screen with a number of options is then shown to the user. It contains all the options along with their brief description to enable the user to understand their functioning and select the proper  option.  
8.	A screen will be provided for user to check his account balance.  
 
9.	A screen will be provided that displays the location of all other ATMs of  same bank elsewhere in the city.  
10.	A screen will be provided for the user to perform various transactions in his account.  
 
The following reports will be generated after each session dealt with in the machine: 	- 
1.	The login time and logout time along with the user’s pin no and account  number is registered in the bank’s database.  
2.	The ATM’s branch ID through which the session is established is also  noted down in the bank’s database.  
3.	Various changes in the user’s account after the transactions, if any, are  reported in the database.  
4.	A printed statement is generated for the user displaying all the transactions he performed.  
 
Other various user interface requirements that need to be fulfilled are as follows:- 
 
 
 
 
Department of CSE, SDBCT, Indore 
Software Engineering & Project Management Lab Manual 
 
 
 The display screen shall be of 10" VGA color type. 
 
 The display screen shall have 256 color resolution. 
 
 The display screen shall also support touch screen facility. 
 
 The speakers shall support Yamaha codecs. 
 
 The keypad shall consist of 16 tactile keys. 
 
 There shall be 8 tactile function keys. 
 
 The keyboard will be weather resistant. 
 
 The transaction receipt shall be 3.1" × 6". 
 
 The statement receipt shall be 4.2" × 12". 
 
 The deposit envelopes shall be 9" long and 4" wide. 
3.1.2 Hardware Interface Requirements  
 
There are various hardware components with which the machine is required to interact. Various hardware interface requirements that need to be fulfilled for successful functioning of the software are as follows:- 
 
 The ATM power supply shall have a 10/220 V AC manual switch. 
 
 	 The ATM card should have the following physical dimensions:- o Width 	-   o Height 	-   o Thickness 	-   
 
 The card reader shall be a magnetic stripe reader  The card reader shall have Smart card option. 
 
 The slot for a card in the card reader may include an extra indentation for the embossed area of the card. In effect it acts as a polarization key and may be used to aid the correct insertion orientation of the card. This is an additional characteristic to the magnetic field sensor which operates off the magnetic stripe and is used to open a mechanical gate on devices such as ATMs.  There shall be a 40 column dot matrix receipt printer. 
 
 There shall be a 40 column dot matrix statement printer. 
 
 The receipt dispenser shall be a maximum of 4" width and 0.5" thickness. 
 
 The statement dispenser shall be a maximum of 5" width and 0.5" thickness. 
 
 The envelope depository shall be a maximum of 4.5" width, 10" length and 0.5" thickness. 
 
 Screen resolution of at least 800X600-required for proper and complete viewing of screens. Higher resolution would not be a problem. 
 
Department of CSE, SDBCT, Indore 
Software Engineering & Project Management Lab Manual 
 
3.1.3 Software Interface Requirements  
 
In order to perform various different functions, this software needs to interact with various other softwares. So there are certain software interface requirements that need to be fulfilled which are listed as follows:- 
 
 
 The transaction management software used to manage the transaction and keep track of resources shall be BMS version 2.0.  The card management software used to verify pin no and login shall be CMS version 3.0. 
 
 Yamaha codecs 367/98 for active speakers. 
 
 The database used to keep record of user accounts shall be Oracle version7.0. 
3.1.4 Communication Interface Requirements  
 
The machine needs to communicate with the main branch for each session for various functions such as login verification, account access etc. so the following are the various communication interface requirements that are needed to be fulfilled in order to run the software successfully:- 
 
 
 The system will employ dial-up POS with the central server for low cost communication. 
 
 The communication protocol used shall be TCP/IP. 
 
 Protocol used for data transfer shall be File Transfer Protocol.(FTP) 
4. System Features  
 
 
 
1. Remote Banking and Account Management 
 
 
Description 
 
The system is designed to provide the user with the facility of remote banking and perform various other functions at an interface without any aid of human  bank teller. The functioning of the system shall be as follows:- 
At the start, the user is provided with a log in screen and he is required 
to enter his PIN NO. and Account details which are then verified by the machine. In case of an unsuccessful attempt a user is asked again for his credentials but the maximum number of attempt given to the user is limited to 3 only, failing which his card is blocked and need to be unblocked by the bank for any future use. 
 
 
  	 
 
 
After a successful log in, the user is presented with a list of language. The user can select any one in the list for interaction with the machine for the entire session. After the language selection the user is also asked whether he wants to fix that language for future use also so that he is never asked for language in future. In addition there is also a facility for the user to switch to any other language during that session. 
 
After the language selection, the user is directed towards a main page 
that displays a set of options/services along with their brief description, enabling the user to understand their functioning. The user can select any of the listed  option and can continue with the transaction. 
The machine also provides the user with a number of miscellaneous 
 	services such as: 
The machine lists a set of operators that are supported by the bank. A 
 	user can clear off his pending mobile phone bills be selecting his operator. 
The machine also has the facility to display a map that marks the 
location of other ATMs of the same bank in the city. This may help the user to look for the ATM nearest to his destination. 
 
At any moment if the user wants to abort the transaction, he is 
provided with an option to cancel it. Just by pressing the abort button he can  cancel all the changes made so far and can begin with a new transaction. 
After the user is finished with his work, for security purpose, he is 
required to log out and then take his card out of the slot. 
 
 
 
 
Validity Checks 
 
In order to gain access to the system, the user is required to enter his/her 
 	correct user id/pin no and account no failing which his card may be blocked. 
The user can access only one account at a time and can enter only one 
 	account no. 
Also if the user is an administrator, he is required to enter his login id in order to access and change the facilities provided by the system. 
 
Sequencing Information 
 
 
 
The information about the users and their account should be entered into the database prior to any of the transactions and the backup be maintained for all account information 
 
 
 
 
 
 
 
 
 	 
 
Error Handling/ Response to Abnormal Situations 
 
If any of the above validation/sequencing flow does not hold true, appropriate error messages will be prompted to the user for doing the needful. 
 
 
2. Receipt Generation 
 
After each transaction user has performed, a receipt is generated that contains all the information about the transaction. The format of the generated receipt is as shown below:- 
 
 
KPM BANK 
 
Branch name/Id 
(address) 
 
Login Time:- 	Date:- 
 
Account No:- User Name:- 
 
TRANSACTIONS: 
 
 
 
 
Logout Time: - 	BARCODE 
 
 
Thank You For your visit. See you soon. 
 
 
 
 
 
 
 
 
 
Page 30
5. Other Non-functional Requirements 
 
 
5.1 Performance Requirements 
 
 
 
The following list provides a brief summary of the performance requirements for the software: 
 
 
 
 
5.1.1 Capacity  
 The ATM shall provide customers a 24 hour service. 
5.1.2 Dynamic requirements  
 
 
 The card verification time must not exceed 0.8 sec. under normal server workload and 1 sec. under peak server workload. 
 
 The pin number verification time must not exceed 0.3 sec. under normal server workload and 0.5 sec. under peak server workload.  Account balance display time must not exceed 2 sec. under normal server workload and 3 sec. under peak server workload.  Account balance transfer time must not exceed 3 sec. under normal server workload and 4 sec. under peak server workload. 
 
 Cash withdrawal transaction time must not exceed 4 sec. under normal server workload and 5 sec. under peak server workload.  Deposit transaction time after insertion of the deposit envelope must not exceed 5 sec. under normal server workload and 6 sec. under peak server workload. 
 
 Receipt printing time after must not exceed 3 sec. under normal server and peak server workload. 
 
 Touch screen and button response time must not exceed 5000ms.  Credit card advance time must not exceed 6 sec. under normal traffic and server and peak traffic and server workload. 
5.1.3 Quality – The primary objective is to produce quality software. As the quality of a piece of software is difficult to measure quantitatively, the following guidelines will be used when judging the quality of the software:  
 
 
 
  	 
 
 
1.	Consistency – All code will be consistent with respect to the 
	 	style. (This is implied when adhering to the standard).  
2.	Test cases – All functionality will be thoroughly tested  
 
 
 
5.2 Software System Attributes  
 
5.2.1 Reliability  
 
 
 The data communication protocol shall be such that it ensures reliability and quality of data and voice transmission in a mobile environment. For example, CDMA. 
 
 The memory system shall be of non-volatile type. 
5.2.2 Availability  
 
 
 The product will have a backup power supply in case of power failures. 
 
 Any abnormal operations shall result in the shutting down of the system. 
 
 After abnormal shutdown of the ATM, the system shall have to be manually restarted by a maintenance personnel. 
 
 There should be no inconsistency introduced in the account during whose transaction the system is abnormally shut down. 
5.2.3 Security  
 
 The system shall be compatible with AIMS security standards.  The system shall have two levels of security i.e. ATM card and pin verification both authenticated by the CMS software. 
 
 The Encryption standard used during pin transmission shall be triple DES. 
 
 The password shall be 6-14 characters long. 
 
 Passwords shall not contain name of customers as they are easy to be hacked. 
 
 Passwords can contain digit, hyphen and underscore. 
 
 User should be provided with only three attempts for login failing which his card needs to be blocked. 
 
 There shall be a security camera installed near the ATM. 
 
 There shall be a secured cash vault with a combination locking system. 
 
 The product cabinet cover shall be manufactured using Fiber glass for security purposes. 
 
 
 
 
 
 
5.2.4 Maintainability  
 
 
 The system components i.e. modem, memory, disk, drives shall be easily serviceable without requiring access to the vault. 
 
 The system should have the mechanism of self-monitoring periodically in order to detect any fault. 
 
 The system should inform the main branch automatically as soon as it detects any error. The kind of fault and the problem being encountered should also be mentioned by the system automatically. 
5.3 Business Rules  
 
The business rules for the software are as follows: 
 
  The Administrator has the authority to fix the rules and regulations and to set or update the policies as and when required. 
	  	The staff at the bank performs the following: 
a.	Making the entries in the system regarding all the details of the bank  account of the user.  
b.	Keeping the bank account of the user updated as soon as changes are  encountered so that the data is in consistent state.  
c.	Blocking or seizing of the account of user on discovery of any illegal  	transaction.  
d.	Unblocking of ATM card that got blocked due to more than three 
	 	unsuccessful login attempt.  
e.	Blocking of a lost/stolen ATM card on complaint of the user, only if he  presents his verification and a FIR filed for that case.  
f.	Constantly monitor all the ATMs in the city to check whether any one of them is encountering any fault.  
g.	Immediately correct any fault discovered in any of the ATM.  
h.	Maintain the backup of all the accounts for reliability purposes.  
i.	Rollback all the changes made in an account during whose transaction an 
	 	ATM got abnormal shutdown.  
  	In case of loss of the ATM card. The user has to lodge a First Investigation Report (FIR) and present its one copy to bank officials for card blocking purposes.   	A log of the following annexure is generated by the system: 
	  	User bank account details. 
  Updations made in the user account along with date, time and the changes made. 
	  	Schedule of fixed assets. 
 
 
 6 Other Requirements None. 
 
 
 
 
 
Appendix A: Glossary 
 
 
 
AIMS 	ATM Information Management System. 
 	 
ATM 	An unattended electronic machine in a public place, connected 
 	to a data system and related equipment and activated by a bank 
 	customer to obtain cash withdrawals and other banking services 
 	 
Braille  
 
 	A system of writing and printing for blind or visually impaired People, in which varied arrangements of raised dots representing letters and numerals are identified by touch. 
 
CDMA 
 
 	 	Code   Division   Multiple   Access,   a   reliable   data  communication protocol. 
 	 
CMS 
 	Card Management Software developed by KPM Bank. 
 
Dial-Up POS 	A message format for low cost communications. 
 	 	 
Internet 
 	An interconnected system of networks that connects computers around the world via the TCP/IP protocol. 
 	 
Smart Card 
 
 	Card without hardware which stores the user’s private keys within a tamper proof software guard. 
Tactile  
Keyboard 
 	 	Special keyboard designed to aid the visually impaired. 
 
 
TCP/IP 	   Transmission Control Protocol/Internet Protocol. 
 
 
 
 
 
Department of CSE, SDBCT, Indore 	Page 34 
Software Engineering & Project Management Lab Manual 
