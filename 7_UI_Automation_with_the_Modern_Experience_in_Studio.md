# ***Target***

- We can describe target as a goal of a activity like a button to click or a text box to type into

- We use target and anchor to identify the correct button, check boxes or dropdown list or the fetch the correct data from te web page/application

- Target is UI element you want to interact

# ***Anchor***
  
- We refer to another UI element as a reference to identify out target

# ***Selection Option Window***

- It allows us to indicate and configure the UI element
  
- When the target highlighted in green, it means the element is identified.
  
- "Pause" option helps us to pause our selection (selection stops for 3 sec.) ***F2***
  
- "Hover able" option, We want to select any UI element, If that is avaible only on hover ***F6***
  
- "Image selection mode" ***F3*** We can use image selection mode for both anchor and target. After pressing F3 then we hold the left mouse button and drag around a region.
  

![Selection_Option_Window-2](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/8f00677e-406f-4011-ac7a-823b2f62fd8a)

# ***Use Application/Browser Activity***

Opens a desktop application or web page to use in UI automation.

- ***Indicate target on screen*** - Indicate the application again.
- ***Highlight Target*** - View the indicated application on your screen surrounded in a box.
- ***Show informative screenshot*** - View a screenshot of the target application or web page.
- ***Remove informative screenshot*** - Remove the screenshot of the target application or web page.
- ***OCR Engine*** - Select one of two options:
- ***Embedded OCR Engine*** - Use the OCR engine embedded in the Computer Vision AI model, namely UiPath Screen OCR.
- ***Custom OCR Engine*** - Use a custom OCR engine. When this option is selected, a panel is added in the activity card where you can drop a different OCR engine activity than UiPath Screen OCR.
  
***Common Section***
  
- ***Continue on error*** : Automation should continue even when the activity throws an error.
- ***Display Name*** : As best practice each activity have a unique name
- ***Timeout*** : Specifies a number of seconds it needs to wait before throwing error(Default value is 30 sec.)

  
***Unified Application Target Section Under the Input Section***

- ***Arguments*** : We can use this property to open a spesific file with the application (For example spesific notepad file path).
- ***File Path*** : It is the full path of executable file to open.
- ***Selector*** : Enables identification of a spesific user interface element through it is adress and attributes.
- ***URL*** : Specifies the URL of the web page to open.If a URL is specified then the file path property is cleared.


***Input/Output Section***
- Input Element - The target element you want to use with this application, stored in an UIElement object. This object can be retrieved from the Output Element property of another UI Automation activity. You can use this property field to pass the target element from a previous activity to this one without having to indicate it again. This field supports only UIElement variables.
- Output Element - Outputs the target element indicated in this activity to an UIElement variable which can then be reused in other activities. This field supports only UIElement variables.


***Misc Section***
- ***Private*** : Related to logging. If it is selected, the values of variables and arguments are no logged at verbose level.


***Options Section***

- ***Close*** : Select when to close the target application after the automation executes all the activities added inside this activity. 'Never' means never close the application. 'IfOpenedByAppBrowser' means close only if the application was opened by the automation. This is the default value. 'Always' means close the application every time.

![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/da4feaee-af8a-4b2c-829c-a781d89c95c2)


- ***Input mode*** : Select which method the Robot should use to interact with the target application. Hardware Events uses the hardware driver to perform the action. This is the slowest method, it cannot work in the background, but it is compatible with all desktop apps. Simulates using accessibility APIs. Recommended for browsers, Java based applications, SAP. Usually more reliable than Hardware Events. Sends all text in a single action. Works even if target app is not in focus. Please test if your target application UI element supports this. Chromium API performs actions using debugger APIs. Works only for Chromium elements. Sends all text in one go. Works even if target app is not in focus. Window Messages simulate using Win32 messages. Recommended for desktop apps. Usually more reliable than Hardware Events. Sends all text in a single action. Works even if target app is not in focus. Please test if your target application UI element supports this. Background runs actions in the background. Tries to use either Simulate or Chromium API where possible, while complex activities (image, native text) run as usual, in the foreground. It is highly recommended to use this method with the Verify Execution feature. Note: Using the Background input mode with Universal Windows Platform applications is not supported, which means applications of this type cannot be automated in the background.

![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/c3aa2c17-a6a3-4622-9f81-8bdc9f022c16)




- ***Open*** : Select when to open the target application for the execution of the automation. 'Never' means never open the application. 'IfNotOpen' means open only if the application is closed. This is the default value. Works only if the File Path or URL fields are populated. 'Always' means open another instance of the application even if one is already open. Works only if the File Path or URL fields are populated.


![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/ffafb307-4a5e-40d0-8131-0676fac281fb)


- ***Resize window*** : Defines whether the application/browser is resized when initialized. 'None' means no resize is applied to the application/browser. 'Maximize' means the application/browser is maximized when initialized. 'Restore to current size' means the application/browser is resized and moved to the position and size it had when indicated, if possible. 'Minimize' means the application/browser is minimized when initialized.

![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/f93940a7-b881-45de-aa65-46403faba800)


- ***Window attach mode*** : Defines where inner activities search for their target elements. 'Application instance' means inner activities search the indicated application instance, including all parent and child windows (alerts, popups, etc). Other instances of the application are excluded. 'Single window' means inner activities search only in the indicated window.

  
![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/a34cdc6a-d14e-458a-815a-4efe297b9d82)



***Options - Browser***

- ***Incognito/private window*** : If selected, opens the new browser session in incognito/private mode. By default, this check box is cleared.

![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/682c3436-8c93-4005-9fc6-82091f388cc4)



- ***User Data Folder Mode*** : The UserDataFolderMode you want to set. It is used to start the browser with a specific user data folder. 'Automatic' means picture In Picture mode uses a different folder than the default mode, automatically generated if UserDataFolderPath is not set. 'DefaultFolder' means uses the default browser folder, no matter if it runs in the main or PIP session. 'CustomFolder' means uses the folder specified in UserDataFolderPath or an auto generated path if UserDataFolderPath is not set.

![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/58f595b2-1298-41a3-84a1-59fe8a72c331)



- ***User Data Folder Path*** - The user data folder that the browser uses. Defaults to %LocalAppData%\UiPath\PIP Browser Profiles\BrowserType if not set.


- ***WebDriver mode*** : Indicates how the WebDriver is used when opening a new browser session. Disabled menas disables the use of WebDriver. WithGUI menas the GUI of the browser is displayed. Headless menas the browser is launched silently, with no GUI.

![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/143d163e-e00f-4852-aa2c-590fedafdf6a)
















