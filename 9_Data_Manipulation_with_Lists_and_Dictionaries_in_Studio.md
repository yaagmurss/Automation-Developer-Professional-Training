# List variable

- List variables are collection type of variables. Meaning that they're part of the System.Collections namespace. 

- Lists, queues, arrays, hash tables, and dictionaries are all part of the System.Collections namespace. 

- They can store numerous elements, like names, numbers, time coordinates, and many others.
  
- It's also possible to have a list within a list.

  

***'List' variable type***



- The List<T>  is a data structure part of the System.Collections.Generic namespace consisting of objects of the same data type.


- The '<T>' represents the type of elements in the list, for example strings or integers.

  
- Each object has a fixed position in the list, and thus it can be accessed by the specific index.

  
- Additionally, it provides methods for searching, sorting, and manipulating lists.



***'IList' variable type***


- The IList is actually an Interface.

  
- In other words, it is a collection of objects that can be accessed individually by their specific indexes.

  
- As in the case of List, the '<T>' represents the type of elements in the list.

  
- The IList<T> generic interface is a descendant of the ICollection<T> generic interface and is the base interface of all generic lists.

  
- Both List and IList type of variables can be initialized with 'new list (of...)'.

  
- For example, if we have a List of IList of String elements type, looking like 'List<IList<String>>',

  
- We can write the following value in the Default value field to initialize it: new List (of IList(of String))

  
- The same initialization value applies for the 'IList<List<String>>' type of variable.



***Differences between List and Arrays***


- Both lists and arrays are collection types of variables.

  
- The array variable enables you to store multiple values of the same type.

  
- UiPath Studio supports as many types of arrays as it does types of variables.

  
- This means that you can create an array of numbers, one of strings, one of Boolean values and so on.

  
- While arrays are fixed-size structures for storing multiple objects, lists allow us to add, insert, and remove items.

  
- If you want to work with a collection that doesn’t have a fixed number of elements, you can use a list instead of an array.


***How to initialize list variables***


- The lists need to be initialized.


- The first way was to create a list type of variable.

  
- Then, we used a Build Collection activity to add items to the list and specify the list variable to hold the items.

  
- The second way was to create a list type of variable, then add the items inside the Default value field.

  
- Then, initialize the list by typing new List of Type from the specified items.



***Value type***



- For numeric, Boolean, DateTime and other value types, the compiler will give them a valid value if we do not explicitly do so.


- For example, Ints initialize to zero by default, DateTimes initialize to DateTime.MinValue by default. In Studio, Strings are also assigned a blank default value, even though they are of the reference type.
bullet


***Reference type***


- Reference type variables, like Lists and Dictionaries, initialize to the object we provide.


- The compiler will not assign a value if we don't.


- This means we need to instantiate an object and assign it to the variable we've just declared.



***To start using reference types like Lists and Dictionaries, we need to go through three steps:***



- We declare a reference variable, for example a List of type String. We provide the name, select the type System.Collections.Generic.List<T> and select String.    


- We initialize an object to be assigned as the initial value for the variable. In our case, we want to start with a List of String object which does not contain values, so we use the expression new List(of String).    


- We assign the object to the new variable (or initialize the variable) either by using the Default value in the Variables panel, or by using an Assign activity.



















