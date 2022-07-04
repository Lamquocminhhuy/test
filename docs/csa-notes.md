<div align="center"> 
  <h1>ServiceNow CSA Notes</h1>
  <h2>Exam Scope</h2>
  
![image](https://user-images.githubusercontent.com/58679620/177077915-ec121251-38a6-407f-845e-9fa89c56b2a0.png)
  
</div>

# I. User Interface & Navigation (20%)

### a. ServiceNow Overview

<details><summary>Click me</summary>
The Now Platform is an Application Platform-as-a-Service (aPaas).

The applications delivered by ServiceNow are divided into four different workflows:

- IT Workflows

- Employee Workflows

- Customer Workflows

- Creator Workflows

\*Now Platform is its multi-instance architecture.
There are three interfaces in Now Platform: Next Experience Unified Navigation (primary way), Now Mobile App (on the go), Service Portal (self-service experience).

> To access to Service Portal: _https://<instancename>.service-now.com/sp_.

Roles contain a collection of permissions.

</details>

### b. Lists and Filters

<details>
<summary>Click me</summary>
Each column in a list corresponds to a field in the table. Each row corresponds to a record in the table.

Context menus provide three different levels of list control:

- list title menu
- list column context menu
- list fields context menu

* Bar Chart and Pie Chart.

* Export can save in serveral formats: Excel, CSA, PDF,...

* The activity stream icon appears in the list title bar.

<hr>

Where do we go in Next Experience to create a new view?

> Configure > List Layout.

Name of the interface we'll use to create a new view?

> List collector.

</details>
<hr>

### c. Forms and Templates

<details>
<summary>Click me</summary>
  
- Forms are displayed in the content frame.

- Forms configured with the activity formatter display a stream of activities
  associated with the record.

- Managing attachments > Click the attachments icon or drag and drop.

- Insert and Stay : when you want to copy a record and just make a few changes.

- Work notes are for internal conversation with those resolving the task.

- Additional comments are for customer visible comments.

- Form Designer, which allows you to add form views, as well as
  add and remove fields on forms.

- The admin or personalize_form role is required to configure forms using Form
  Designer.

<div align="center">

![image](https://user-images.githubusercontent.com/58679620/177075648-e4f6aa8a-c9df-4694-9d3b-b890ea4e9243.png)

  <p>Form Designer vs Form Layout Interface</p>
  
</div>

<div align="center"> 
  
![image](https://user-images.githubusercontent.com/58679620/177075502-dd39f269-95a7-4c24-bac8-275d48c1059b.png)
  
  <p> The list collector interface allows you to select multiple items from an Available list and remove items from a Selected list</p>
  
</div>

</details>
  
# II. Collaboration (20%)
  
### a. Task Management

<details>
<summary>Click me</summary>

Automation repeatable processes

> Save time.
> The Task table is one of ServiceNow’s core tables.

![image](https://user-images.githubusercontent.com/58679620/177078749-cbd05c0f-7805-4b4d-b811-7bfeb5f8786d.png)

Task specifics functionality:

- Approvals: can be generated to a list of Approvers, either manually or automatically, according to approval rules. Approvals can be incorporated into workflows or can stand alone.
- Assignment: rules can automatically assign tasks to users or groups, ensuring that tasks are handled by the most appropriate team members.
  > All > System Policy > Rules > Assignment.
- Service Level Agreements: can track the amount of time that a task has been open, to ensure that tasks are completed within an allotted time.

Activity Stream appear in Notes tab.

Visual Task Boards (VTB) to collaborate on tasks in real-time with group members, create personal to-do lists, and more.

There are three types of Visual Task Boards:

- Guided: can be created from a list and use the values of a specified field (e.g. State) as lanes. Tasks in the list are updated when cards are edited or change lanes on the Visual Task Board.
  > updates automatically.
- Flexible: also created from a list, but lane changes do not update underlying task data.
- Freeform: can act as your personal organizer to manage individual tasks of any kind. Lane changes do not update underlying task data.

```
Lanes allow you to sort records by field values or other user-defined values.
```

Work notes are only visible to those who can view the task, Additional comments are only visible to the customer (caller), and Activities are read-only record entries.

Which of the following are ways to collaborate with team members on Tasks?

> User presence, Activity Stream, Work Notes.

  </details>
  
### b. Notifications 
  
<details>
<summary>Click me</summary>
Emails, meeting notification, text messages.
  
Sys admin can define notification in All > System Notification > Notifications. 
  
  ![image](https://user-images.githubusercontent.com/58679620/177081169-f9607874-437c-4d90-9056-82b3e1795016.png)

```
  When to send, Who will received, What it will contain.
```

To customize the content message go to Show Notification Scripts.

</details>
  
### c. Reportings
<details>
<summary>Click me</summary>
_Now Platform Report Designer_ to build reports.

> After you create a report, it appears in the All > Reports > View/Run module under the My reports list.

_Performance Analytics (PA)_ allows users to create dashboards with widgets to visualize data over time in order to identify areas of improvement.

Keys:
Enter a Report name, Source type, and a Table or a Data source > Data Tab.

Select the report visualization format > Type Tab.

Define the report grouping > Configure.

Choose colors, title, and chart properties > Style.

  </details>

### d. User Administration

 <details>
<summary>Click me</summary>
   A good practice is to assign roles to groups rather than to users.
   
   More about impersonate a user: [Docs](https://docs.servicenow.com/bundle/sandiego-platform-administration/page/administer/users-and-groups/concept/c_ImpersonateAUser.html#c_ImpersonateAUser)
  </details>
  
# III. Self-Service & Process Automation (20%)
### a. Knowledge Management
  
<details>
<summary>Click me</summary>
 - Informations store in Knowledge Base (KB).
 
 - Self-service > Knowledge Base or go to Service Portal /sp.

- Helpful ?, rating a star, leave a comment.

- End users can post questions and answer in **Social Q&A**.

- **The Most Useful** item in the Knowledge Management Service Portal displays articles that have the highest percentage of users marking them helpful.

</details>

### b. Service Catalogue

<details>
<summary>Click me</summary>

- Request items.
- Access in All > Self-Service > Service Catalog.
- Catalog Builder use to create or edit catalog items, view the available catalog items, templates, recently updated.
- **Administrators** can manage all and scripting, **Catalog administrators** also can manage all except scripting.
- Products and services in the service catalog organized in **Categories and Subcategories**.
- **Flow and Workflow** fulfillment process for a service catalog item.

```
task-based records
```

</details>

### c. Workflows/Flow Designer

<details>
<summary>Click me</summary>
- Flows automate business logic.
- Flow Designer bulding and enabling process automation, **without code**.
- To access All > Process Automation > Flow Designer.
- Flow Designer trigged by Record-based, Application-based, Schedule-based (Date).
- Actions are operations executed by Flow Designer, such as looking up a record, updating a field value, requesting an approval, or logging a value.
- Flow Designer Data : data pills 
</details>
  
 # IV. Introduction to Development (10%)
## a. Scripting

<details>
<summary>Click me</summary>

- Plugins are software components that provide additional optional features and functionalities within a ServiceNow instance.
 > Access: Sytem Definition > Plugins.

- Client-side [see more](https://lamquocminhhuy.github.io/servicenow-dev-notes/client-side-scripting.html) and Server-side Scripting [see more](https://lamquocminhhuy.github.io/servicenow-dev-notes/server-side-scripting.html).

- A UI policy action can change fields on a form to be madatory (required), visible/hidden, or read-only.

- UI Policy and Client Script run client-side.

</details>


## b. Migration and Integration

<details>
<summary>Click me</summary>

- An update set tracks changes to applications and platform features, then groups them together so they can be moved from one instance of ServiceNow to another. 

- Update Sets work by writing changes from tracked tables to the Customer Update [sys_update_xml] table. (newest change overide the old one).
- Merge Update Sets the most recent change will be the one moved to the merged update set.
- **Data records, Dashboard** are not captured in an update set.
- To create an Update Set : All > System Update Sets > Local Update Sets. Then click New.

Standard integrations for ServiceNow include:
*	Login (Single Sign-On)
*	LDAP
*	Communications
*	Monitoring
*	Systems Management

> **Intergation Hub**


</details>

## c. Development

<details>
<summary>Click me</summary>

- App Engine Studio (AES) build apps even faster using app templates for pre-built solutions.
- The Automated Test Framework (ATF) enables you to create and run automated tests to confirm that your instance works after making a change.
- Delegated developers are non-administrator users and groups that are assigned one or more permissions to develop applications (without having the admin role).
- To delegate All > System Applications > My Company Applications. select Developer (invidual) or Groups.

```
  The Guided Applicatio Creator is used to begin the creation of an application.
```
</details>
