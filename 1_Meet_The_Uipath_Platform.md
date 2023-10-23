***Components of the uipath platform***  
 &rarr; Studio,   
 &rarr; Orchestrator,     
 &rarr; Robot,   
 &rarr; Assistant.  

 ----------------  

***Uipath Robots***

A software robot is an execution agent that runs automations built with the Studio family and then published as packages either locally, or to Orchestrator. 

 &rarr; ***Attended robots***  

They're digital helpers for human users. They work on the same machines as us humans, during the same hours. They're triggered directly by humans (usually through UiPath Assistant) or by an event related to what the human user does. For example, opening an application or receiving an email.  
UiPath Assistant is the component that provides a friendly interface to interact with attended robots. It is the tool that we use to easily access, manage, and run automations. 

 &rarr; ***Unattended robots***  

These are meant to work non-stop, with as little input from human users as possible. They're deployed on separate machines and their jobs are triggered exclusively from Orchestrator.
Their interactions with human users are typically handled with as little disruption as possible, by creating and sending requests for human input or validation as tasks.
While these await to be processed, unattended robots can continue their work by picking up other jobs.
When human input is finally provided, unattended robots can resume their work on the process.  

***Automation Cloud Robots***  

Automation Cloud Robots (ACRs) are SaaS robots hosted in the UiPath Automation Cloud that let you quickly run automations without building or managing your own unattended Robot infrastructure. They come in two flavors: 

&rarr;  ***VM Automation Cloud Robots.***  
- Access to a fully customizable Windows virtual machine and set up UiPath Robots to run any job in a matter of minutes.  
  
&rarr;  ***Serverless Automation Cloud Robots (Linux based cloud robots)***
- Run background, cross-platform projects easily without worrying about infrastructure setup. So, you're able to provision, manage and scale these robots from Automation Cloud. In other words, UiPath takes care of everything

&rarr;  ***Test Robots*** 
- These robots can be deployed to execute tests on-demand, continuously, and at scale. Here are some of the characteristics of a test robot:
- Purpose built for testing workflows, activities, and applications.
- Provides flexibility in managing and reusing test cases across projects. 
- Enables activity level unit testing out-of-the-box.

----------------  

***Uipath Orchestrator***


Orchestrator, the heart of automation management, is a web application that allows managing, controlling, and monitoring the robots and the automations. 
With Orchestrator we can deploy, trigger, measure, provision, track, and ensure the security of every robot in the organization. 
Orchestrator also functions as a repository for libraries, reusable components, assets, and processes used by robots or by developers.


***The main capabilities of Orchestrator are:***
- ***Provisioning:*** creates and maintains the connection with robots.
- ***Control and license distribution:*** enables the creation, assignment and maintenance of licenses, roles, permissions, groups, and folder hierarchies.
- ***Automation storage and distribution:*** allows the controlled storage and distribution of automation projects, assets, and credentials, as well as large files used in automations.
- ***Running automation jobs in unattended mode:*** enables the creation and distribution of automation jobs in various ways, including through queues and triggers.
- ***Monitoring:*** allows monitoring of jobs and robots and stores logs for auditing and analytics.

----------------  

***Uipath Task Capture***


UiPath Task Capture is a process documentation automation tool.
It exports screenshots, step by step details, and detailed annotation in a PDD or XAML.



***Uipath Process Mining***


Process Mining is visualization and analysis of event logs with the help of algorithms and mathematical procedures. 
Uipath Process Mining tool discovers automation-ready pain points, deviations, and inefficiencies across processes.


***Uipath Task Mining***


Uses Al to automatically capture and analyze the day-to-day tasks performed by the employees, 
Construct the data-driven process maps, and suggest automation ideas with the highest ROI potential. 


***Uipath Studio***


Uipath Studio is for developers to build automation projects with basic coding konowledge.
It is an drag and drop technology for development.


***Uipath Studio X***


Enables business users to rapidly automate without the need for developer resources or coding, making automation accessible to all.

***Uipath Document Understanding***


Uses AI-enhanced skills to extract data and interpret documents. It can process different document types and formats, including tables, handwriting, signatures, and checkboxes. Uses human validation to confirm extracted data if needed, handle exceptions, and train models to improve their accuracy over time.


***Uipath Integrations***


Leverages API integrations with leading enterprise applications, built and supported by UiPath and backed by partners.


***Uipath Marketplace***


Enables consumers to discover and use trusted, enterprise-grade RPA content. 


***Uipath Test Manager***


Governs and monitors the quality of the automations. It facilitates test planning and execution, requirements, and defect traceability, includes comprehensive test reporting, and seamlessly adapts to environments with out-of-the-box integrations.


***Uipath AI Center***


Facilitates the automation of more complex or  cognitive processes with RPA robots learning Al skills.
Enables you to deploy your own Al skills or pre-trained Al skills developed by UiPath or UiPath Al technology partners.


***Uipath Insights***


Using powerful embedded analytics you can measure, report, and align RPA operations with your specific KPls and strategic business outcomes. 


***Uipath Data Service***


A powerful no-code data modelling and storage tool that ensures seamless access, enterprise-grade security, and scalability of the data.


***Uipath Assistant***


Lets all the users interact with robots right on their desktops through an easy-to-use launchpad


***Uipath Action Center***


Brings humans in the loop to make required decisions when the automated processess require exceptions, escalations, and approvals



***Uipath Apps***


Enables you to build, use, and share elegant business apps that interact with your automations



***Uipath Chatbots***


Connects chatbots with UiPath processes for the fulfillment of user requests without writing a single line of code.



 ----------------  
 

***Steps to set up your attended user and run your first job***

As the Automation Cloud account admin:

- Invite the new user to Automation Cloud and include them in the Automation Developers group.
- Allocate the Automation Developer - Named User license type.
- Go to Orchestrator, search for the newly added user, and assign the Robot role.

As the attended user:
- Check your mailbox and accept the invitation from the administrator.
- Login to Automation Cloud.
- On the Home tab, click Download UiPath Studio.
- Run the Studio installer.
- Sign in to Automation Cloud from Studio.
- Choose the Studio profile.
- Create a new automation process in Studio.
- Add a Message Box activity and input the desired message.
- Publish the project to Orchestrator.
- Open UiPath Assistant, install, and run a job for the newly added process.

------------------

**NOTES**
- Larger enterprise customers may choose an on-premises deployment and the integration with Active Directory. In this case, the user groups would be imported in the host tenant, where licenses would also be allocated. 
- For Community accounts, the first user would also be the admin on the Automation Cloud and the Orchestrator service.
- UiPath Automation Cloud is our cloud platform, hosting our cloud products and services.
- Cloud Orchestrator is a service hosted in Automation Cloud. 
- Users and groups need to be created first in Automation Cloud. 
- Then you'll be able to add them and configure their permissions and licenses in Orchestrator. 
- The Automation Users and Automation Developers groups are by default added in Orchestrator.

----------------


***Uipath Hardware and Software Requirements***
![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/5bf5e0a7-1c0d-4e7e-ae25-957c794fd131)

![resim](https://github.com/yaagmurss/AdvancedRPADeveloperCertificationTrainingNotes/assets/52479605/cfa5b1ed-ce08-4228-8a84-16114eb280fd)

----------------  
