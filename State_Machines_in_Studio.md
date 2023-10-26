# WorkFlow Design Lesson overview


***Flowchart*** 

- Which allows for visual representation and decision-making in complex scenarios.

- Flowcharts provide enhanced flexibility in connecting activities and present workflows in a visually appealing two-dimensional format. Their free-form nature makes them well-suited for displaying decision points in a process. 

- However, caution must be exercised, as the use of arrows that can point anywhere may resemble unstructured GoTo programming statements, potentially leading to chaotic interweaving of activities, especially in larger workflows. 


***Sequence***  

- Layout for simpler linear flows.
  
- Sequences exhibit a straightforward linear representation, flowing seamlessly from top to bottom, making them ideal for uncomplicated scenarios where activities follow a sequential order, such as procedural workflows involving step-by-step data entry, form submissions, or document processing. 

  
***State Machines*** 

- Layout for managing states and transitions.

- Some processes are better expressed as interconnected states which are executed again and again whenever necessary. A set of activities are performed in each state and then a condition is evaluated to determine what state to transition to next. 

- In Studio, the State Machine workflow layout lets you design event-driven processes based on a finite number of states and transitions. This layout should be used for high level project organization for complex and continuous processes. For this reason, State Machines are often used in Main.xaml for RPA frameworks like the Robotic Enterprise Framework.





