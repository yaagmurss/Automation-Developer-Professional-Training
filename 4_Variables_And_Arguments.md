***Variables*** 

Basic units of storing information

***Name Of A Variable***

It should be as descriptive as possible to make your automation easy to read by other developers and to save time. 
While not the only option, we recommend:Using PascalCase for variable names. 
PascalCase is a naming convention in which the first letter of each word in a variable is capitalized. Eg: ItemValue, LastName.

***Type Of A Variable***
It defines what kind of data is stored in the variable. 
In UiPath, the data type is declared when the variable is created.  
The dropdown field provides quick access to the most used data types (seen below), but there are many more options available to you, if you select "Browse for Types". 
- Boolean
- Int32
- String
- Object
- System.Data.DataTable 
- Array of [T]
- Browse for Types

***Scope of A Variable***

The part of the workflow in which the variable is called by name. 
A typical automation project consists of different workflows, nested, or connected in different ways.
The scope of a variable is defined by the name of the workflow in the automation project. 

***Default***
Inital value of a variable. It is change through workflow.
It is not mandatory.


***Data Types***
Most of them are borrowed from Visual Basic.NET language.

***String***
Used to store text

***Numeric***
Used to store numbers

- Int32
- Long
- Double

***Boolean***
Used to store two values (true(1) false(0))

***Collection***
Used for handling and processing complex data 
- Array(used to store multiple values of the same data type. The size (number of objects) is defined at creation.)
- List (used to store multiple values of the same data type, just like Arrays. Unlike Arrays, their size is dynamic.)
- Dictionary (used to store objects in the form of (key, value) pairs, where each of the two can be of a separate data type.)

***DataTable***
Act as a database or a simple spreadsheet with rows and columns.

***DateAndTime***
- DateTime (Used to store specific time coordinates )
- Timespan (Used to store information about a duration )

***GenericValue***

- This is a UiPath proprietary variable type that can store any kind of data, including text, numbers, dates, and arrays. 
This type is mainly used in activities in which we aren't sure what type of data we'll receive, yet in general, using this is temporary.

***What are some business scenarios in which you will use GenericValue?***
- Data is extracted from a UI field and forwarded to another workflow without processing.
- Two versions of the same Excel file are being compared column by column. The columns are different in terms of data type, the only relevant thing is which entries have changed. 


***What is a workflow?***

- A workflow represents a relatively small piece of an automation project,typically executing a specific part of the process. 
- Once built, it can be reused across different projects.

- UiPath Studio provides you with predefined workflow layouts to suit all the needs of a fast and reliable automation process.

- ***The workflow layouts are:***
- Sequences
- Flowcharts
- State Machines
- Global Exception Handler

- The fastest, most reliable, and useful way of automating a process is to break it down into smaller bits. 


- This allows for independent testing of components, enables team collaboration, and component reuse. 


- Hence, most of the automation projects require the use of multiple workflows that come together to provide a solid business automation solution.



***What is it?***

- An array variable or argument is a type that enables storing multiple values of the same data type

- StrArray = {"John", "Paul", "George", "Ringo"}
- StrArray(0) = "John" 

- Arrays are the most common example of a collection with a fixed size, the one at creation.
- Think of it as a group of elements with a size that is defined at creation, and where each item can be identified by its index.
- Arrays are usefull where we need to store multiple values of the same type



***Conversion methods of Data Types***

***Convert.ToString Method***
StrVar = Convert.Tostring(IntVar)

***Convert.ToInt32***
IntVar = ToInt32(StrVar)
IntVar = CInt(StrVar)
IntVar = ToInt32(DblVar) 

***Double.ToString Method***
StrVar = DblVar.ToString

***Double.Parse Method***
DblVar = Parse(StrVar) 

***Boolean.ToString Method***
StrVar = Convert.Tostring(BoolVar)

***Convert.ToBoolean Method***
BoolVar = ToBoolean(Int32) 

***Convert DateTime To String***
DateTime.Now 
Gets a DateTime object that's set to the current date, and time on this computer, expressed as the local time.

ToString(DateTime) 
Converts the value of the specified DateTime to its equivalent string representation.




















