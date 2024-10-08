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
======================================================
- Go to `Project Settings` -> `Boards` -> `GitHub connections`.
- Click on `Connect your GitHub account`.
- You will be taken to GitHub, where you will have to authorize Azure DevOps.
- Select the repository you want to connect with Azure DevOps.
- Then you can see the repository in the `GitHub connections` tab.
------------------------------------------------------
## Azure Queries
======================================================
- `Queries` are useful to find certain data around your work, items in your sprints and get the results in a required format.
- You can go to `Boards` -> `Queries` and create a new query.
- *Bulk Update, Assign or reassign* - Queries are used to do bulk update, assign, or reassign work items or task.
- *Email list of work items*
- *Reporting Feature*
------------------------------------------------------
## Azure Repos
======================================================
- Similar to `GitHub`, `Azure Repos` is a place where you can store your code.
- `Store and Collaborate`.
- All the features in GitHub are available in `Azure Repos`.
- `Official Definition` - **Get unlimited, cloud-hosted private Git repos and collaborate to build better code with pull request and advanced file management.**
------------------------------------------------------
## What is version control?
======================================================
- `Version Control System (VCS)` **is nothing but a tool to manage your code at a centralized place and track all the changes you or team has done.**

### Why do we need version control?
- **Collaboration**
- **Storing Versions (Properly) Saving a version of your project after making changes.**
- **Restoring Previous Versions**
- **Understanding What Happened**
- **Backup**
### Types of Version Control
- **Git** - Distributed Version Control System
- **TFVC** - `Team Foundation Version Control` - Centralized Version Control System

### Git and GitHub
- `GitHub` is a platform where you can store your code and collaborate with your team.
- `Git` is a version control system that is used to manage your code.
------------------------------------------------------
## Setup Development Environment
======================================================
### What is required?
- **Install Git**
- **Install Visual Studio Code**
- **GitHub Account**
- **Azure DevOps Account**
- **Azure Repos**

### Create/Import Repository
- Go to `Repos`.
- On top, you can click and you will get options to create a new repository or import a repository.

------------------------------------------------------
## Some Terminologies - 04
======================================================
### Understanding Git Terminology
- **Branches** - Copy of `main` or some other branch.
- **Commit** - Snapshot of the project's currently staged changes.
- **Pull Request** - Request to merge changes from one branch to another.
------------------------------------------------------
## CI/CD
======================================================
- **CI/CD** stands for `Continuous Integration/Continuous Deployment`.
- **CI** - `Continuous Integration` is a development practice that requires developers to integrate code into a shared repository several times a day. It simply means merging of code from different branches in one single branch and making sure that code integration is happening smoothly and flawlessly.
- **CD** - `Continuous Delivery/Deployment` is a practice that allows you to automate the process of deploying code to production. When your code is merged and ready, you are going to build it. The pipeline is going to build it and it will create some `artifact` (a package that is ready to be deployed). `CD` basically means building the required artifact and deploying it to the production environment.
- **Pipelines** - Pipelines are used to automate the process of building, testing, and deploying code. This is the place where `CI/CD` happens. So merging of code and creating the artifact and deploying it to the production environment is done using `Pipelines`.
------------------------------------------------------
## Azure Pipelines
======================================================
- **Microsoft Definition** - *Build, test and deploy with `CI/CD` which works with any language, platform and cloud. Connect to GitHub or any other Git provider and deploy continuously.*
- What are the benefits of `Azure Pipelines`?
    - **Execution of Continuous Integration takes place.**
    - **Builds or Run Jobs/task when code is submitted.**
    - **Build Agent - helps to build the code.**
    - **Outputs a build artifact(.zip file, .jar file, .exe file etc.)**
    - 
### Types of Pipelines
- **Build Pipeline** - Used to build the code.
- **Release Pipeline** - Used to deploy the code.

### Creating Pipeline
- Go to `Pipelines` -> `Create Pipeline`.
- You will be asked to choose the repository.
- You can choose `GitHub` or `Azure Repos`.
- You will be asked to choose the template.
- You can choose `Starter Pipeline` or `YAML`.
- You can choose `Starter Pipeline` if you are new to `Azure Pipelines`.
------------------------------------------------------
## CI/CD Using GitHub Actions
======================================================
### GitHub Actions
- **GitHub Actions** is a feature of GitHub that enables the creation of custom automated workflows triggered by specific events in a repository.
- These workflows are defined in `YAML` file and consist of jobs, steps, and actions. A workflow can be configured to run when events like code pushes, pull requests, issues, etc. occur.
- Each workflow contains one or more jobs, each job contains a series of steps, and these steps utilize reusable actions or custom commands to perform tasks such as building, testing, deploying or notifying stakeholders.
======================================================
### GitHub Actions: Workflow
- **Workflow** is a defined sequence of automated steps and actions that are executed whenever specific events occur in a GitHub repository.
- These events can range from pushing new code, creating pull requests, opening issues or even scheduled events.
- Workflows allow you to automate various tasks such as building, testing, deploying, and notifying stakeholders. Making it easier to manage and maintain your software projects lifecycle.
======================================================
### Understanding GitHub Actions YAML File
```yaml
name: name-of-workflow

on:
    push:
        branches: ["main"]
    
jobs:   # Jobs are the main building blocks of a workflow
    build:
        runs-on: self-hosted    # Runner environment will be maintained by user

        steps:  # Steps are the individual tasks that will be
        - uses: actions/checkout@v4
        - name: Set up Node.js
          uses: actions/setup-node@v2
          with:
            node-version: '14'
        - name: Install dependencies
            run: npm install
        - name: Build
            run: npm run build
        - name: Test
            run: npm test
```
- All the YAML files are stored in `.github/workflows` directory.
======================================================
### Setup Self-Hosted Runner
- Go to `Settings` -> `Actions` -> `Runners`
- And go through the steps provided according to your OS.
- That simple.
======================================================

