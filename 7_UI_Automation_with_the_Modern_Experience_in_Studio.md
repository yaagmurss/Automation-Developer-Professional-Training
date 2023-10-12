***Target***

- We can describe target as a goal of a activity like a button to click or a text box to type into

- We use target and anchor to identify the correct button, check boxes or dropdown list or the fetch the correct data from te web page/application

- Target is UI element you want to interact

***Anchor***
  
- We refer to another UI element as a reference to identify out target

***Selection Option Window***

- It allows us to indicate and configure the UI element 
- When the target highlighted in green, it means the element is identified.
- "Pause" option helps us to pause our selection (selection stops for 3 sec.) ***F2***
- "Hover able" option, We want to select any UI element, If that is avaible only on hover ***F6***
- "Image selectiom mode" ***F3*** We can use image selection mode for both anchor and target. After pressing F3 then we hold the left mouse button and drag around a region.

![Selection_Option_Window-2](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/8f00677e-406f-4011-ac7a-823b2f62fd8a)

***Use Application/Browser Activity***
- Opens a desktop application or web page to use in UI automation.
- ***Common Section***
- Continue on error : Automation should continue even when the activity throws an error.
- Display Name : As best practice each activity have a unique name
- Timeout : Specifies a number of seconds it needs to wait before throwing error(Default value is 30 sec.)
- ***Unified Application Section under the Input Section***
- Arguments : We can use this property to open a spesific file with the application (For example spesific notepad file path).
- File Path : It is the full path of executable file to open.
- Selector : Enables identification of a spesific user interface element through it is adress and attributes.
- URL : Specifies the URL of the web page to open.If a URL is specified then the file path property is cleared.
- ***Input/Output Section***
- Input/Output element is used to identify the target/UI element to perform an action.
- We can pass the value to these either through a variable or with an argument of type "UIElement".
- We use the input/output element property to identify the target/UI element instead of selector property. For any UI automation activity, the selector and input/output element properties, both cannot be filled at the same time.
- ***Misc Section***
- Private : Related to logging. If it is selected, the values of variables and arguments are no logged at verbose level.
- ***Options Section***
- Close : Resposible for selecting when to close the target application after the automation executes all the activities added inside(Never-Always-IfOpenedByAppBrowser).
- Input Mode : Based on our selection behaviour of the automation changes
- Open : This propety is responsible for deciding when to open the target application for the execution of the all the activities in the Do container(never-always-IfNotOpen)
- Resize Window : Resize window when initialized or when it is opened. (None-Maximize-RestoretoDesingTime-Minimize)
- Window Attach mode : Application Instance(It searches the application instances for its UI element including all parent and child windows(alerts-pop ups etc.)). Single Window(activity search only in the indicated window)
- ***Options-Browser Section***
- 















  ![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/fe9c673d-f17a-4100-9b29-e0b88d9f842a)
























