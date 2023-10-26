# ***Data manipulation*** 

Process of modifying, structuring, formatting, or sorting data to make it easier to read, use and manage.

***Consistent Data*** : 

- Data collected from various sources might not be well organized. 
- Data manipulation can ensure that data is structured and stored consistently.


***Data Integration*** : 

- In many cases, data is stored in collected and stored in multiple locations. 
- Data manipulation methods enable the integration of data from various sources providing a consolidated view of the data.


***Data Visualization*** : 

- Data manipulation helps structure data in a format that supports effective visualization. 
- Organizing and summarizing data helps create meaningful dashboards, charts, or reports that communicate insights clearly and concisely. 


***Data Analysis*** : 

- To conduct data analysis or modelling, data needs to be prepared in a suitable format. 
- Data manipulation facilitates in transforming and organizing data to make it compatible with analysis technique.


***Properties*** : 

- Attributes of an object or an aspect of its behavior. 
- For example, the string class contains two properties: Chars (returns the Char object at a specified position in the current String object) and Length (returns the number of characters in the current String object). 
- For example, based on the previous example, Username.Length returns 8. 


***Methods*** : 

- Actions that an object can perform. 
- Methods often have parameters that qualify how the action is performed. 
- For example, Username.Replace("John","Jack") returns "Jack Doe". 


***String.Concat***

- Concatenates one or more instances of string or string representation of objects.
- Expression: String.Concat (VarName1, VarName2)
- Output datatype: String

***Contains***

- Checks whether a specified substring occurs within a string and returns either true or false.
- Expression: VarName.Contains (“text”)
- Output datatype: Boolean

***String.Format***

- Converts the value of objects to strings and inserts them into another string.
- Expression: String.Format(“{0} is {1}”, VarName1, VarName2)
- Output datatype: String

***IndexOf***

- Returns the index position of the first occurrence of a specified character or a substring. 
- Expression: VarName1.IndexOf(“a”)
- Output datatype: Int32

***LastIndexOf***
- Returns the index position of the last occurrence of a specified character or a substring.
- Expression: VarName1.LastIndexOf("author")
- Output datatype: Int32

***String.Join***
- Concatenates the elements in a collection using the specified separator and displays them as a String.
- Expression: String.Join(“|”, CollVarName1)
- Output datatype: String

***Replace***

- Replaces all the occurrences of a substring in a string.
- Expression: VarName.Replace (“original”, “replaced”)
- Output datatype: String

***Split***

- Splits a string into substrings using the specified separator.
- Expression: VarName.Split(“|“c)(index)
- Output datatype: Array of String

***Substring***

- Extracts a substring from a string using the starting index and the length.
- Expression: VarName1.Substring(startIndex, length)
- Output datatype: String

***The Text to Left/Right activity***

- Retrieves the text to the left and right of the first occurrence of the indicated subtext.

***The Modify Text activity***

- Updates a text value using modifications including find and replace, trim, and combining (concatenating) with another text value.

***The Change Type activity*** 

- Changes the type of a variable to another type.  


# Regular Expression

***Regular Expression (RegEx, or regexp)*** is a specific search pattern that can be used to easily match, locate and manage text. However, creating RegEx expressions may be challenging. UiPath Studio contains a RegEx builder that simplifies the creation of regular expressions.

***Typical uses of RegEx include***

- Input Validation

- String Parsing

- Data Scraping
  
- String Manipulation

***Matches***

    \d Matches any digit character (0–9)
    \D Matches any character that is not an digit (0–9)
    \w Matches any word character (A-Z, a-z, 0–9, _ ) (alphaNumeric and underScore)
    \W Matches anything that is not a word character (spaces, ?, *, + …)
    \s White space (space, tab, newLine)
    \S Matches anything that is not White space (space, tab, newLine)
    \b Word Boundry
    \B Not a word Boundry
    ^ Beginning of the string
    $ End of the string
    . Matches anything except lineBreaks

***Character Set***

    [1–7] Numbers between 1 to 7
    [1234567] Numbers between 1 to 7
    [a-z] Lower case numbers
    [A-Z] Upper case numbers
    [A-Za-z] Lower case + upper case numbers

***Exact Numbers***

    \d{11} Contains 11 digit
    [] Matches caharacter in brackets
    [^] Matches caharacter not in brackets
    | Either Or
    () Group

***Quatifier***

    * ==> 0 or More
    
    + ==> 1 or More
    
    ? ==> 0 or One
    
    {3} ==> ExactNumber
    
    {3,4} ==> Range Of Number

    


***Look Ahead and Look Behind***



      .(?=u) ==> Choose a character continue with “u”
      
      .(?!u) ==> Choose a character that is not continue with “u”
      
      (?<=q). ==> Choose a character there is “q” before
      
      (?!=q). ==> Choose a character there is not “q” before
      Meta Characters



_____________________________________________________________

    . [ { ( ) \ ^ $ | ? * +

    - If we want to find MetaCharacters like “.”
    - We need to use escape character “\\.”

_____________________________________________________________
































