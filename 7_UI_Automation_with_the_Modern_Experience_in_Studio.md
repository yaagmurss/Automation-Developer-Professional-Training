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
















  ![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/fe9c673d-f17a-4100-9b29-e0b88d9f842a)






***Use Application/Browser***

- Opens a desktop application or web browser page to use in UI automation.

- After you drag and drop the activity in the workflow and indicate the application or web page to use, add the activities to be performed inside the Use Application/Browser activity. If the application is not already open, it opens when the project is executed.

- This activity is compatible with Object Repository.

- Click Indicate Application to identify the application by moving the mouse to its window and clicking it. If the target is a browser web page, navigate to the page before you indicate the application.
- After you indicate the target, manage the target by clicking Menu and selecting the following options:
- ***Indicate target on screen*** - Indicate the application again.
- ***Highlight Target*** - View the indicated application on your screen surrounded in a box.
- ***Show informative screenshot*** - View a screenshot of the target application or web page.
- ***Remove informative screenshot*** - Remove the screenshot of the target application or web page.
- ***OCR Engine*** - Select one of two options:
- Embedded OCR Engine - Use the OCR engine embedded in the Computer Vision AI model, namely UiPath Screen OCR.
- Custom OCR Engine - Use a custom OCR engine. When this option is selected, a panel is added in the activity card where you can drop a different OCR engine activity than UiPath Screen OCR.


***Properties panel***

***Common***

- Continue on error - Specifies if the automation should continue even when the activity throws an error. This field only supports Boolean values (True, False). The default value is False. As a result, if the field is blank and an error is thrown, the execution of the project stops. If the value is set to True, the execution of the project continues regardless of any error.

- Display name - The name displayed for the activity in the Designer panel. A display name is automatically generated when you indicate a target.

- Important: The display name of the Use Application/Browser activity is also used as a reference that points to the application or browser that is being targeted. After indicating the target, unless manually set, the display name is automatically changed to the following format:

- Timeout - Specify the amount of time (in seconds) to wait for the activity to be executed before throwing an error. You can also choose a predefined value from the drop-down menu: 10 (s), 20 (s), 30 (s). The default value is 30 seconds.

- Note: When indicating a window in a Remote Desktop environment, the timeout default setting is set to 60 seconds.

***Input***

- Unified Target Application - Expand this category to configure the following settings:
- Arguments - If the application is not a web browser, you can specify parameters to pass to the target application at startup. You can use this property to open a specific file with the application. For example, if the target application is Acrobat Reader, you can open a specific workbook by providing the full path to the file. To open the file C:\Sample.pdf, enter "C:\Sample.pdf". Certain application types are automatically identified and autofill the Arguments property, such as Java apps, Office Suite apps, Adobe Acrobat, or Windows File Explorer.
- File path - If the application is not a web browser, specifies the full path of the executable file to open. If a file path is specified, the URL property is cleared.
- Note: When the path defined in the File path field is dynamic, clicking Indicate target on screen in child activities generates an error if the target application is not already open.    Selector - An XML fragment that stores the attributes of a user interface element.
- URL - If the application is a web browser, specifies the URL of the web page to open. If a URL is specified, the File path property is cleared.

***Input/Output Element***
- Input Element - The target element you want to use with this application, stored in an UIElement object. This object can be retrieved from the Output Element property of another UI Automation activity. You can use this property field to pass the target element from a previous activity to this one without having to indicate it again. This field supports only UIElement variables.
- Output Element - Outputs the target element indicated in this activity to an UIElement variable which can then be reused in other activities. This field supports only UIElement variables.

***Misc***

- Private - If selected, the values of variables and arguments are no longer logged at Verbose level. This field supports only Boolean (True, False) values. The default value is False.

***Options***

- Close - Select when to close the target application after the automation executes all the activities added inside this activity:
- Never - Never close the application.
- IfOpenedByAppBrowser - Close only if the application was opened by the automation. This is the default value.
- Always - Close the application every time.

- ***Input mode*** - Select which method the Robot should use to interact with the target application:

- Hardware Events - Uses the hardware driver to perform the action. This is the slowest method, it cannot work in the background, but it is compatible with all desktop apps.

- Simulate - Simulates using accessibility APIs. Recommended for browsers, Java based applications, SAP. Usually more reliable than Hardware Events. Sends all text in a single action. Works even if target app is not in focus. Please test if your target application UI element supports this.

- Chromium API - Performs actions using debugger APIs. Works only for Chromium elements. Sends all text in one go. Works even if target app is not in focus. For more details, check out this page.

- Window Messages - Simulate using Win32 messages. Recommended for desktop apps. Usually more reliable than Hardware Events. Sends all text in a single action. Works even if target app is not in focus. Please test if your target application UI element supports this.

- Background - Runs actions in the background. Tries to use either Simulate or Chromium API where possible, while complex activities (image, native text) run as usual, in the foreground. It is highly recommended to use this method with the Verify Execution feature.
- Note: Using the Background input mode with Universal Windows Platform applications is not supported, which means applications of this type cannot be automated in the background.    Open - Select when to open the target application for the execution of the automation:
        ***Never*** - Never open the application.
        ***IfNotOpen*** - Open only if the application is closed. This is the default value. Works only if the File Path or URL fields are populated.
        ***Always*** - Open another instance of the application even if one is already open. Works only if the File Path or URL fields are populated.

-Resize window - Defines whether the application/browser is resized when initialized.
        ***None*** – No resize is applied to the application/browser.
        ***Maximize*** – The application/browser is maximized when initialized.
       ***Restore to current size*** – The application/browser is resized and moved to the position and size it had when indicated, if possible.
        ***Minimize*** – The application/browser is minimized when initialized.
    ***Window attach mod*** - Defines where inner activities search for their target elements.
    ***Application instance*** - Inner activities search the indicated application instance, including all parent and child windows (alerts, popups, etc). Other instances of the application are excluded.
    ***Single window*** - Inner activities search only in the indicated window.

***Options - Browser***

- Incognito/private window - If selected, opens the new browser session in incognito/private mode. By default, this check box is cleared.
- User Data Folder Mode - The UserDataFolderMode you want to set. It is used to start the browser with a specific user data folder.
        ***Automatic*** - Picture In Picture mode uses a different folder than the default mode, automatically generated if UserDataFolderPath is not set.
        ***DefaultFolder*** - Uses the default browser folder, no matter if it runs in the main or PIP session.
        ***CustomFolder*** - Uses the folder specified in UserDataFolderPath or an auto generated path if UserDataFolderPath is not set.
    ***User Data Folder Path*** - The user data folder that the browser uses. Defaults to %LocalAppData%\UiPath\PIP Browser Profiles\BrowserType if not set.


- WebDriver mode - Indicates how the WebDriver is used when opening a new browser session. The following options are available:        Disabled - Disables the use of WebDriver.
- WithGUI - The GUI of the browser is displayed.
- Headless - The browser is launched silently, with no GUI.



***Cross-platform configuration***

- The name of the activity in cross-platfrom projects is Use Browser and it can be used to automate only web browsers.

- Work in scope - Choose the browser tab rendering the web application to automate.
- URL - The URL of the web application. The value is automatically filled after choosing the tab.
- Requires Authentication? - Enabled multi-factor authentication. For more details, check out the UI Automation Browser Connection page.

***Additional options***

***Timings***

- Timeout - Specify the amount of time (in seconds) to wait for the activity to be executed before throwing an error. You can also choose a predefined value from the drop-down menu: 10 (s), 20 (s), 30 (s). The default value is 30 seconds.
- Continue on error - Specifies if the automation should continue even when the activity throws an error. This field only supports Boolean values (True, False). The default value is False. As a result, if the field is blank and an error is thrown, the execution of the project stops. If the value is set to True, the execution of the project continues regardless of any error.


- Open - Defines whether to open the target application before executing the activities in it.
        Always - Open the browser window every time.
        If not open - Open a new browser window, if none matches the selector and the URL. This is the default value.
        Never - Never open the browser window.
- Close - Defines whether to close the target application before executing the activities in it.
        Always - Close the browser window every time.
        If opened by Use Browser - Close only if the browser window was opened by the Use Browser activity. This is the default value.
        Never - Never close the browser window.
- Input mode - The method used to generate keyboard and mouse input.
        Chromium API - Performs actions using debugger APIs. Works only for Chromium elements. Sends all text in one go. Works even if target app is not in focus.
        Simulate - Simulates the action using accessibility APIs. Works for browsers. Sends all text in a single action. Works in the background (even if the target application is not in focus).
- Incognito/private window - If selected, opens the new browser session in incognito/private mode. This field only supports Boolean values (True, False). The default value is False.

- User data folder mode - The user data folder mode you want to set. It is used to start the browser with a specific user data folder.
        Automatic - Picture In Picture mode uses a different folder than the default mode, automatically generated if User data folder path is not set.
        Default folder - Uses the default browser folder, no matter if it runs in the main or PIP session.
        Custom folder - Uses the folder specified in User data folder path or an auto generated path if User data folder path is not set.

- Setting the browser user data folder is only available for Chrome, Edge Chromium and Firefox.
- User data folder path - The user data folder that the browser uses. Defaults to %LocalAppData%\UiPath\PIP Browser Profiles\BrowserType if not set.

***Target***

- Selector - List of attributes used to find a particular browser window.

***Input/Output***

- Input element - The UI element on which the activity is executed, stored in an UIElement object. This field supports only UIElement objects. This object can be obtained from the Output Element property field of other UI Automation activities.
- Output element - Outputs a target UI Element and stores it in a UIElement object, which can be further used to target the same element with other activities.



















