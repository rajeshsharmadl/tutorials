# DevOps
***
A culture (not a tool, technology or methodology) of close integration between development, QA & operation teams for smooth development, test and deployment with agility.

> It is an integration of people, process and products to provide maximum value ratio to customer.

> **DevOps Portal**
> [https://dev.azure.com](https://dev.azure.com)

#### SDLC (Software Development Life Cycle)

| Business Team | Development Team      | Operations Team              |
| ------------- | --------------------- | ---------------------------- |
| Planning      | **Dev**elopment       | **Op**eration**s**           |
|               | Code -> Build -> Test | Deploy -> Operate -> Monitor |

Each DevOps culture defines and provides tools to manage tasks, code, tests and deployment in their own way. Once you setup a DevOps environment, development and deployment teams along with stake holders benefit from it. It brings agility to entire SDLC.

#### DevOps Services

- Boards - Write stories, tasks, bugs, progress, to-do, etc. using agile board/kanban board
- Repos - Manage code versioning using git/tfs
- Pipeline - Automation (CI/CD) is available
- Test Plans - Automates/Manual testing can be managed
- Artifacts - Collection of packages available from private/public repos required during development for working of project

VSTS (Visual Studio Team Services)	|	Azure DevOps Services
----------------------------------	|	---------------------
Work								|	Boards
Code								|	Repos
Build & Release						|	Pipelines
Test								|	Test Plans
Packages							|	Artifacts

#### Organization
It is a collection of related projects. Each DevOps account can have multiple organizations. Organizations can also be made as/for subgroups as it is easy to separate and handle large number of projects. Each organization have its owl URL e.g. https://dev.azure.com/{organization-name}.

#### Project
It is a collection of related tasks. This is where entire product development is handled by a particular team and it provides repositories for code versioning and place for people to plan, track progress and collaborate. A project can be public or private. It contains a team by name of '{project-name} Team' by default when we create a project but we can add other teams also.

##### Public Project
- Visible to everyone
- No login required to access
- Unique URL
- Mostly used for open source projects
- Unlimited public projects inside any organization

##### Private Project
- No public visibility
- Authorised access only
- Unique URL
- Mostly used for non-public development

#### Team
A group of people responsible for development of project(s) and include developers, quality analysts (testers), scrum master, PO, deployer or any stakeholder who has any interest in the project. A single project can contain multiple teams. Only administrators can make changes to team.

#### Board
Boards are used to defining tasks/work items, report bugs, track progress, share user stories, reporting, etc.

**Uses of Board**
- Manage and track work
- Provides a clear picture of tasks undertaken/in progress/completed by team members
- Allow access to stakeholders to view progress of development
- Manage scrum, sprint
- Manage backlog
- Various reports

**Who will work on Board:**
- Entire team
- Development team will work related to their tasks, bugs, features, etc.
- Product owner (PO) will manage backlog
- Stakeholder will see the progress
- Scrum master will get various reports pertaining to progress of project

**Types of Board**
DevOps has four types of processes or project namely Basic, Agile, Scrum and CMMI and user can select any type while creating the project. Type of board i.e. work items and work flow available will depend on what user selects.

**Work Flow**
Work flow is various stages of tasks of product development. Multiple tasks can exist during a product development and each task can be on different stage of progress. Each project type or work item type will have different stages depending on project type.

**Work Item**
Work item is a unit of work which needs to be done in a product. Multiple items co-exist during product development.

**Backlog**
A collection of work items to be developed in the future. It is used to quickly define a requirement which is yet to be started.

**Types of Backlog**
- Product Backlog - It is an ordered list of all the work items needed to be done in a product
- Sprint Backlog - Sprint is a planned period of time during which a work item is to be completed and presented for review. It is a collection of work items in ToDo state. We can assign work items and set estimated sprint duration for completion of items.

**Kanban Board**
Kanban is a japanese word for 'Visual Signals' and these signals are used to display several units in a way that user can identify each item state by looking at the unit's visual state. Various colors, positions or other designs are used in Kanban board to make it easy for user to understand.

#### Basic Process

**Work Flow in Basic process**

ToDo -> In Progress -> Done

**Work items in Basic process**

- Epic - It consists of functionalities as large which are to be included into the product e.g. Membership
- Issue - An epic may contain multiple issues like bug, user story, improvement, etc. e.g. Membership may need login, signup, forget password, reset password, etc. requirements
- Task - For each issue, we can have multiple tasks depending on the nature of the issue. Each task will have a defined work of a particular nature. e.g. for completing each of the above issues, we need to create/change database tables, develop methods for each of the issue, consume the methods at relevant places, etc.

**Fields/Properties of a work item with Basic process**
- Title - Test containing 255 characters or less. It can be modified later
- AssignedTo - Team members are assigned the work items so that the development progress can be tracked by all the team members including the assignee. If there is a change/bug/query related to work item completed, allowed members can add the change/bug/query in the work item and change the status so that assigned member can resolve the issue which he can track by using the kanban board
- State - Represents the current state of work item i.e. ToDo, Doing or Done
- Reason - Reason is needed which changing the wotk item state
- Area - A path associated with product or team
- Iteration - Represents the sprint or iteration in which a work item is to be completed
- Description - Details about the work item
- Effort - A relative estimate of time required to complete a work flow
- Discussion - Used to raise a discussion or add a comment or ask information
- Start Date - Date on which work item s beginning
- Target Date - Date till which a work item is supposed to complete
- Tag - Additional very short detail associates to the work item
- Priority - Provide the level of urgency about the work item from 1 to 4. 1 says that item is very urgent and to be looked asap and prouct can not be shipped without successfull resolution. 2 says that item is not urgent and can be looked after but product can not be shipped withput successfull resolution. 3 says that resolution of work item is optional depending on resources available, time required and risk involved. 4 says that resolution is not necessary
- Attachment - Add an attachment to the work item
- History - It shows all the changes done to the work item
- State Graph - It shows the changes in state using a graph

#### Agile Process

**Work flow in Agile process**
- Agile process follows different work flow for different work items:
? User Story work flow - Work flow in agile process has multiple steps as: New Use Story -> Active (When implementation starts) -> Resolved (Code complete and user tests passed) -> Closed (Acceptance tests passed)
? Bug work flow - Work flow for a bug in agile process has following steps: New Bug -> Active (when approved and working starts) -> Resolved (when user make the necessary changes/correction) -> Closed (when bug is verified to be corrected)
? User task work flow - User task work flow has following steps: New Task -> Active (when work started) -> Closed (when task completed)

**Work items in Agile process**
- Epic - It contains major work items needed in the product. It represents a business initiative. It is considered inside a portfolio backlog.
> Feature - These are the shippable component of a software. These are enhancements needed in the product to improve user experience. An epic may contain multiple features.
> User Story - These are the user requirements. It is considered inside a product backlog.
> Task - It is the smallest unit of work needed to be done for accomplishment of work item.
> Test Case - Test cases are used by QA for proper testing of the product. 
> Issue - It is any thing which is needed in the product but is not part of standard work flow and can not be clubbed with work items.
> Bug - It is a wrong implementation or incorrect piece of code.

CMMI Process (Capability Maturity Model Integration)
----------------------------------------------------

Work flow in CMMI process
? CMMI wok flow is as follows: Proposed (items to work on) -> Active (when work started) -> Resolved (when task is com



