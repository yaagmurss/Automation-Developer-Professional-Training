***UI AUTOMATION***

- User interface or graphical user interface automation (UI Automation) refers to the process of interacting with graphical elements within applications by simulating mouse and keyboard controls.

***Major GUI frameworks***

- Win32
- WPF
- HTML
- Java

***UI Automation is built upon seven key concepts***

1) UI Automation activities (Activities tell robot what to do)
2) Activity properties (Properties control how the Robot exectes an activity)
3) Targeting methods (Targetting methods help the robot to identify the correct UI element to perform the action)
4) Input and output methods (Input and output methods tell the robot what technology to use to send input to get output from interface)
5) Recorders (The recorder will help you develop UI automation by following your manual interaction with a GUI step by strp and tranlating it into a sequence of studio activities)
6) Scraping Wizards (Scaping wizard help you extract structured data automatically)
7) The object repository (It allows developers to store UI element identifiers in a repository, fine tune them and share them with colleagues for more faster UI automation development and project update)
8) AI Computer Vision (AI Computer vision is an AI skill that enables all uipath robots to see every element on a computer screen)

**UI Automation activities***

- Containers (These are activities that identify the browsers or apps the process needs to interact with. All activities included within a Container will execute on the same application. Some examples are Open Browser, Attach Browser, Open Application, or Use Application/Browser.)
- Input Activities (These activities send input to UI elements. They can be used to click, check, type into, send hotkeys, and so on.)
- Output Activities (These activities get information from GUI Elements. They can instruct the Robot to get the text by using various methods, get structured data, or get the UI Elements containing images.Example "Get text activity")
- Synchronization Activities (They help you create triggers based on the UI behavior, thus enabling the Robot to execute certain actions when specific events occur on a machine. Example: "on element appear activity")

***Activity properties***

- Properties determine how the robot performs an action.

- DelayAfter/DelayBefore (How many milliseconds the robot waits before or after executing the activity.)
- ContinueOnError (Will an exception encountered while executing the activity be thrown or ignored? if the element isn't found, will robot throw an error and stop the execution, or will it ignore it and continue?)
- Target (Provides several properties related to identifying the target UI Element.)
- Timeout (How many milliseconds will the Robot try to perform an action on an UI element. )
- SendWindowsMessages/Simulate Type	(What input method do we use for input activities.)
- Output (It Stores the output of the activity in the form of variables.)

***Targeting methods***

- Targeting methods are a subset of Properties. They provide several ways to identify the UI element the Robot will be interacting with. 
- Selectors 
- Fuzzy Selectors 
- Image  
- Native Text

***INPUT METHODS***

***Hardware events***

- Clicking 
- Typing
- Compatible with all applications
- Does not work in the background
- The attended user cannot touch the mouse during the automation

***Send Window Messages***

- Replays the window message that the target app receives when the mouse/keyboard is used

***Simulate***

- Uses the technology of the target application (API level) to end instructions
- It is the fastest targeting method 
- Works in background
- Users can work on other activities during the execution of the automated process

***ChromiumAPI***

- It is a browser automation input method based on the Devtools protocol
- It allows direct communication with the browser, in turn fewer communication channels and thus improved automation reliability
- Works in the background
- Users can work on other activities during the execution of the automated process.

***OUTPUT METHODS***

***Full Text***

- The FullText method is the default method and good enough in most cases. It is the fastest, it can extract hidden text, it has 100% accuracy, and can work in the background. 

***Native***

- The Native method is compatible with applications that use Graphics Design Interface (GDI), the Microsoft API used for representing graphical objects. It doesn’t extract hidden text and it cannot work in the background; and just like FullText, it doesn’t support virtual environments.

***OCR***

- OCR (or Optical Character Recognition) is the only output method that works with virtual environments and with “reading” text from images. Its technology relies on recognizing each character and its position. On the other hand, it cannot work in the background, it cannot extract hidden text, and its speed is by far the lowest.


***Design experiences***

- Modern Design Experience

- Classic Design Experience

***We can change the design experience based on the requirement, in two ways***

- Change the default design experience at Studio level.
![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/25bdf95b-04b4-4d36-86fe-1f9d88cca580)


- Change the design experience at Project level. 
![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/25415e8b-cff0-4568-af91-18bd337f946a)

***The key differences between the modern design experience and the classic design experience are based on the following key concepts***

- UI Automation activities

- Activity properties

- Targeting methods

- Input methods

- Recorders and Scarping wizards

- The object repository

***NOTE***

- Note that modern activities only work within containers, while classic activities can be configured to work without containers as well. 

- Modern and Classic activities have slightly different properties because of different targeting methods and Activity behaviors. We'll learn more about this in the following lessons.

- Both design experiences use input methods (Hardware events, SendWindowMessages, and Simulate). A new input method, ChromiumAPI, is used in the modern experience.

- Modern experience ==> The App/Web and Computer Vision recorders are available.

- Classic experience ==> The Basic, Desktop, Web, Image, Native Citrix, and Computer Vision recorders are available.

- Modern experience ==> The Table Extraction wizard is available for data scraping.

- Classic experience ==> The Data Scraping and Screen Scraping wizards are available.

- Full text output method belongs both experience

***Modern Experience***

- Targetting methods : Native Text
- Targetting methods : Unified Target(cycles through all of the available targeting methods)
- Scraping wizard : Table Extraction 
- Recorders : App/Web and Computer vision
- It is default option unless updated
- Object repository
- Input Method : Chromium API
- Activities : UI Activities only work with containers

***Classic Experience***

- Recorders: Basic, Desktop, Web, Image, Native Citrix and Computer vision 
- Targetting methods : Mostly selectors
- Scaping wizard : Data scraping and screen scraping
- Activities : UI Activities can work without containers

