# List variable

- List variables are collection type of variables. Meaning that they're part of the ***System.Collections*** namespace. 

- Lists, queues, arrays, hash tables, and dictionaries are all part of the System.Collections namespace. 

  

***List variable type***


- The ***List<T>***  is a data structure part of the ***System.Collections.Generic*** namespace consisting of objects of the same data type. The '<T>' represents the type of elements in the list, for example strings or integers.

  
- Each object has a fixed position in the list, and thus it can be accessed by the specific index. Additionally, it provides methods for searching, sorting, and manipulating lists.



***IList variable type***


- The ***IList*** is actually an Interface. In other words, it is a collection of objects that can be accessed individually by their specific indexes.

  
- As in the case of List, the '<T>' represents the type of elements in the list. The ***IList<T>*** generic interface is a descendant of the ***ICollection<T>*** generic interface and is the base interface of all generic lists.

  
- Both List and IList type of variables can be initialized with 'new list (of...)'. For example, if we have a List of IList of String elements type, looking like ***List<IList<String>>***. We can write the following value in the Default value field to initialize it: ***new List (of IList(of String))***





***Differences between List and Arrays***



- Both lists and arrays are collection types of variables.

  
- The array variable enables you to store multiple values of the same type. UiPath Studio supports as many types of arrays as it does types of variables. This means that you can create an array of numbers, one of strings, one of Boolean values and so on.

  
- While arrays are fixed-size structures for storing multiple objects, lists allow us to add, insert, and remove items.

  
- If you want to work with a collection that doesn’t have a fixed number of elements, you can use a list instead of an array.


***How to initialize list variables***


- The lists need to be initialized. The first way was to create a list type of variable. Then, we used a Build Collection activity to add items to the list and specify the list variable to hold the items.

  
- The second way was to create a list type of variable, then add the items inside the Default value field. Then, initialize the list by typing new List of Type from the specified items.





# Dictionary Variable 

- Dictionary variables (Dictionary<TKey, TValue>) are collection type of variables of (key, value) pairs, in which the keys are unique.


***Methods for working with dictionary variables***

- ***Initialization***:  We can add new Dictionary(Of String, String) inside the Default value field in the Variables panel or Data Manager panel for the respective variable, or use an Assign activity to assign the value to the variable within the workflow.
  

- ***Adding Key-Value Pairs*** :  VarName.Add(Key, Value) adds an item to an existing dictionary variable. Because Add doesn't return a value, we use the Invoke Method or Assign activity.
  

- ***Removing Keys*** : VarName.Remove(Key) removes an item from the dictionary variable. It can be used in an Invoke Method activity.
  

- ***Retrieving*** :  VarName.Item(Key) returns the Dictionary item by its key. VarName.Count returns an Int32 value of the number of Dictionary items.
VarName.ContainsKey(Key) checks if the item with the given key exists in the dictionary variable and returns a Boolean result.



***Collection-specific activities***

- Build Collection
- Remove From Collection
- Exists in Collection
- Append item to Collection
- Merge Collections
- Filter Collections
- Collection to Data Table 

















