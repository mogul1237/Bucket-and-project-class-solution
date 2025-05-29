# Bucket-and-project-class-solution

Download Here: [Bucket and project class solution](https://jarviscodinghub.com/assignment/bucket-and-project-class-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

You are required, but not limited, to turn in the following source files:
Assignment4.java (Download this file and use it as your driver program for this assignment)
Project.java
Budget.java
Requirements to get full credits in Documentation
description need to be included at the top of each file/class.
A description of each method is also needed. Some additional comments inside of methods (especially for a “main” method) to explain code that are hard to follow should be written. You can look at the Java programs in the text project to see how comments are added to programs.
Skills to be Applied
In addition to what has been covered in previous assignments, the use of the following items, discussed in class, will probably be needed:
Classes
Instance Objects
Accessors/Mutators(Modifiers) methods
Visibility Modifiers (Access specifier) – public, private, etc.
Encapsulation concept
Aggregation relationship between classes
DecimalFormat or NumberFormat class in java.text package
Program Description
Class Diagram:

Assignment #4 will be the construction of 2 new classes and a driver program (the class containing a main method).
Budget class
The Budget class describes the budget of a Project. It has following attributes:
Attribute name Attribute type Description
initialFunding double initial funding of a project
spending double spending of a project
currentBalance double current balance of a project
The following constructor should be provided to initialize each attribute:
public Budget(double funding)

This constructor initializes initialFunding to the parameter value, spending to 0.0, and currentBalance is computed as initialFunding-spending.
The following method should be provided to add any additional spending. If the parameter value is positive and is less than or equals to currentBalance, it should be added to spending, and currentBalance should be re-computed as initialFunding-spending, and the method should return true. Otherwise, the method should not change any value and return false.
public boolean addSpending(double amount)
The following method must be defined:
public String toString()
The toString() method constructs a string of the following form:
Budget:\n
Initial Funding\t$0.00\n
Spending\t$0.00\n
Current Balance\t$0.00

where the first dollar amount is initialFunding value, the second is spending value, and the third is currentBalance. You can use NumberFormat class to format the above three numbers. Note that those values can be some other values other than $0.00
Project class
The Project class describes a project that people can participate in. It must have the following attributes:
Attribute name Attribute type Description
projName String name of a project
projNumber String number of a project
projLocation String location of a project
projBudget Budget budget of a project
The following constructor should be provided to initialize each attribute:
public Project(double amount)
This constructor initializes all strings to “?” and the project number to 0, and instantiates an object of Budget (i.e., call the constructor of the Budget class to create an object of Budget), using the parameter value (amount).
The following accessor methods should be provided to get the attributes:
public String getName()
public int getNumber()
public String getLocation()
public Budget getBudget()
The following mutator methods should be provided to change the attributes:
public void setName(String aName)
public void setNumber(int aNumber)
public void setLocation(String aLocation)
The following mutator method should be provided to change the budget. It should call addSpending method of the Budget class:

public boolean addExpenditure(double amount)
The following method must be defined:
public String toString()

The toString() method constructs a string of the following format:
\nProject Name:\t\tConstruction Project\n
Project Number:\t\t15\n
Project Location:\tPhoenix\n
Budget:\n
Initial Funding\t$0.00\n
Spending\t$0.00\n
Current Balance\t$0.00\n\n

You can make use of the DecimalFormat or NumberFormat class in java.text package to format initialFunding, spending, and currentBalance, having two digits after the a decimal point “$0.00”.
Assignment4
(Note that this part is already done in the Assignment4.java file that is given to you. This explains each functionality of this class.)
In this assignment, download Assignment4.java file by clicking the link, and use it for your assignment.You do not need to change Assignment4.java file. You only need to write Budget.java and Project.java files.
The following is the description of Assignment4 class.
The driver program will allow the user to interact with your other class modules. The purpose of this module is to handle all user input and screen output. The main method should start by displaying the following menu in this exact format:

Choice\t\tAction\n
——\t\t——\n
A\t\tAdd Project\n
D\t\tDisplay Project\n
Q\t\tQuit\n
R\t\tAdd Expenditure\n
?\t\tDisplay Help\n\n
Next, the following prompt should be displayed:
What action would you like to perform?\n

Read in the user input and execute the appropriate command. After the execution of each command, re-display the prompt. Commands should be accepted in both lowercase and uppercase.
Add Project
Your program should display the following prompt:
Please enter the project information:\n
Enter a project name:\n
Read in the user input. Then the following prompt:
Enter a project number:\n
Read in the user input. Then the following prompt:
Enter a project location:\n
Read in the user input. Then the following prompt:
Enter a project initial funding:\n
Read in the user input, then use the constructor of the Project class to initialize the object, project1, and set the values read from the user input, using the mutator (setter) methods of the Project class.
Note that there is only one Project object in this assignment. Thus when “Add Project” option is selected more than once, the new one overwrites the old Project object.
Display Project
Your program should display the Project information using the toString method of the Project class. The toString method is used together with System.out.print method.
Quit
Your program should stop executing and output nothing.
Add Expenditure
Your program should display the following prompt:
Please enter any additional expenditure:\n
Read in the user input and update the budget of the project accordingly by calling the addExpenditure method of the project object. If it returns false, then it should display the error message: The entered expenditure is not accepted.
Display Help
Your program should redisplay the “choice action” menu.
Invalid Command
If an invalid command is entered, display the following line:
Unknown action\n
Input
The following files are the test cases that will be used as input for your program (Right-click and use “Save As”):
Test Case #1
Test Case #2
Test Case #3
Test Case #4
Output
The following files are the expected outputs of the corresponding input files from the previous section (Right-click and use “Save As”):
Test Case #1
Test Case #2
Test Case #3
Test Case #4
Error Handling
Your program is expected to be robust to handle all test cases.
