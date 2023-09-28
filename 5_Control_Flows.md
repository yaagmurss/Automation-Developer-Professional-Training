***The workflow layouts***

-Sequence (Activities in sequences are easier to read and maintain)
-Flowchart (Use flowcharts when decision points and branching are needed  )
-State Machine ( that uses a finite number of states in its execution)
-Global Exception Handler.

***The most common control flow statements are ***
- If, 
- While, 
- Do While, 
- For Each, 
- Switch, 
- Parallel.

***For Each loop***
- Performs an activity or series of activities on each element of an enumeration.
- Iterates through each element in the collection.
- Exits upon completion of processing of each item in the collection.

***While loop***
- Executes contained activities while the condition is True.
- Iterates as long as the condition is met.
- Exits upon checking if the condition is false.

***Switch***
- Useful when we need at least three potential sources of action.
- Uses a condition that is not boolean. But enables the selection of one choice out of multiple, based on the value of a specified expression. 
- Workflow design with multiple nested If-Else replaced by switch activity is easy to follow.
- By default, switch activity uses an integer argument in the Case Value section in Studio.

***If***
- Useful only with two potential courses of action.
- Uses a condition that is boolean in nature.
- Workflow design with multiple nested If-Else looks cluttered and difficult to follow.
- If statement uses an integer or character.