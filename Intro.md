# DevOps
------------------------------------------------------
## What is DevOps?
======================================================
In a typical software product lifecycle, following steps are followed:

**Development**
1. Plan         
2. Code
3. Build
4. Test
5. Deployed

**Operation**
1. Managed
2. Monitored
3. Feedback -> Back to Plan

- First the product is planned -> Then the developers code it using a VCS (such as Git) -> Then the code is built using tools (such as Maven) -> Then the code is tested -> Then the code is deployed (on Cloud Services such as AWS) using tools like (Chef/ Ansible) -> **From here on operation part begins** -> The deployed code is managed (managing the servers) -> Application is monitored (using tools such as Nagios) -> Feedback is taken from the monitoring and the product is sent back to planning phase.
- Development and Operation both are smoothened and eased by using correct choice of action and using appropriate automation tools.
- Making the development and operation work together and making the process of software development and deployment faster and easier is called DevOps.
- **So, DevOps is basically a culture or concept which eases or foster this lifecycle by automating it using right set of tools and right practices.**
------------------------------------------------------
## Azure DevOps (Introduction)
======================================================
- Azure DevOps is a Software as a Service (SaaS) platform from Microsoft that provides an end-to-end DevOps toolchain for developing and deploying software.
- Azure DevOps provides developer services to support teams to plan work, collaborate on code development, and build and deploy applications.
- Everything is automated and everything is in one place.
------------------------------------------------------
## Creating Organization
======================================================
- Go to [Azure DevOps](https://dev.azure.com/) and sign in.
- Click on **Start Free** tab.
- Create a new organization, by filling in the details.
- After creating the organization, you will be taken to the dashboard.
------------------------------------------------------
## Some Terminologies - 01
======================================================
### Azure DevOps Services
- **Boards** - Agile tools to plan and track work.
- **Pipelines** - Build, test, and deploy with CI/CD that works with any language, platform, and cloud.
- **Repos** - Unlimited cloud-hosted private Git repos for your project.
- **Test Plans** - All in one planned and exploratory testing solution.

### Integrations and Extensions
- **Slack**
- **Trello**
- **Campfire**
- **GitHub** etc.
------------------------------------------------------
## Creating Project
======================================================
- Click on **New Project**.
- Give it a `Name` and `Description`.
- Choose `Visibility` as `Public` or `Private`.
- Choose `Version Control` as `Git` or `TFVC`.
- `Work Item Process` as `Basic` or `Agile` or `Scrum` or `CMMI`.
- Click on **Create**.
------------------------------------------------------
## Some Terminologies - 02
======================================================
### Azure Boards Components
- **Work Items** - Tasks, bugs, user stories, etc.
- **Boards** - Kanban boards to visualize work items.
- **Backlogs** - List of work items.
- **Sprints** - Time-boxed iterations.
- **Dashboards** - Widgets to monitor progress.

### Board Work Process
- **Basic** - When you want simplest model that uses Issues, Tasks & Epics to track work.
- **Agile** - Whe your team uses Agile planning methods, including Scrum, and tracks development and test activities separately.
- **Scrum** - When your team uses Scrum planning methods and tracks development and test activities separately.
- **CMMI** - `Capability Maturity Model Integration` , when your team follows more format project methods that require a framework for process improvement and and auditable record of decisions.

------------------------------------------------------
## Changing the default work process
======================================================
- Go to `Project Settings` -> `Overview` -> `Process`.
- Click on the current process, scroll down and under `Boards` click `Process`
- You will see the current process, selected `(default)`.
- You can change the process to `Agile` or `Scrum` or `CMMI`.
- Click on `Save`.
------------------------------------------------------
## Inviting users to your project
======================================================
- On the project homepage, You can see `Invite` tab, (As of now, 25 August 2024), on the top right corner.
- Click on `Invite`.
- Enter the email address of the user you want to invite.
- Click on `Add`.
- The user will receive an email invitation.
- You can see current members in the `Members` tab, in `Summary`.
------------------------------------------------------
## Creating Work Items
======================================================
- Click on `Board` tab.
- You will see all the options of work items 
    - `Boards`
    - `Backlogs`
    - `Sprints`
    - `Queries`
    - `Delivery Plans`
    - `Analytics views`
- Click on `Boards`.
- By default you will get to a `Kanban board`.
- We can use this board to track our issues, tasks, user stories etc using the `Kanban board`. It has all the features of a typical Kanban board.
------------------------------------------------------
## Some Terminologies - 03
======================================================
- `Sprint` - A sprint is a short, time-boxed period when a scrum team works to complete a set amount of work.
- `Themes` - A bigger goal that you/organization wants to achieve. A **Theme** can be divided into **Epics** or **Initiatives**.
- `Epics` - A big chunk of work that has one common objective. An **Epic** can be divided into **Features**. **Epics** usually correspond to time duration of 3-6 months.
- `Features` - Features are certain tasks that are part of an **Epic**. **Features** can be divided into **User Stories**. **Features** usually correspond to time duration of weeks.
- `User Stories` - User stories are small, specific, and independent tasks that are part of a **Feature**. **User Stories** usually correspond to time duration of days. **Stories** can be sub-divided into **Tasks**.
- `Tasks` - Tasks are the smallest unit of work. **Tasks** usually correspond to time duration of hours.
------------------------------------------------------
## Connect Azure Boards with GitHub
