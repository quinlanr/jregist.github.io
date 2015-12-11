# Code I/O Meeting Summary 
**_Dec. 8-9, 2015, Atlanta, GA_**

##Digital Project Process##

Most of our time was spent talking through our process; while other topics such as platform and application architecture received attention, in one way or another nearly everything that we talked about comes back to process. For example, if someone is developing on a Mac and the website will ultimately reside on a Windows server running IIS, our process must include a way to assure that the website is tested on IIS early enough to make sure that any issues that come up can be resolved prior to launch. 

In general, our process has the following as the key components:

- Track project requirements and scope, platform and frameworks using a standard form,
- List all these projects on a web application called our Project Clearinghouse,
- Use Jira to track tasks, bugs and progress on apps under development,
- Use GitHub as our code repository,
- Use a Mongo (or other document) database and SQL Server,
- Use Node and relevant JS libraries as a platform for backend,
- Use Angular and other relevant JS libraries for the frontend,
- Use Materialize is our CSS Framework,
- Other libraries: D3, Neo need to be better understood,
- A QA / QC process including front-end and back-end testing is required prior to deploying an application. 

The following sections will define these in more detail. 

### Project Kickoff, Requirements Form and the Project Clearinghouse

To understand the requirements of the apps that we are being asked to build, we must create a standard process that guides the initial stages of the project and requires that relevant information about the project is written down and shared. To share information about those projects with one another and the firm most easily, we will create a web form for us to use to enter the information. All new projects will be required to complete the Project Requirements form before they can become a project and work can begin. Once projects are completed and the site has gone live, the content entered into this Requirements form (along with additional information) will be accessible via an application that we can use to keep track of the status of the site, its maintenance needs, future projects that will update, extend or replace the application. We are calling this site the Project Clearinghouse. 

TO DO: We will create a very simple 2-page website allowing people us to enter project requirements, technology and JS frameworks used, location where it currently resides, etc. and then to list the project among other projects of its type. We will take into account elements from Murali's ['Development Framework Worksheet'](http://./content/files/DEV_FORM.pdf) and [Dylan's Project Specification form](http://pwc01gisdata/specs/specs.html). 

### Use Jira to Track Tasks on all our Projects

We have begun using Jira and have assigned the Code I/O team to development projects currently in progress. We will begin including the development teams in India to use Jira beginning next week (12/14/2015). By using a single repository for all our projects, each of the Code I/O team members will be able to see their tasks on each project at a glance. Joel will serve initially as Scrum Master, making sure that projects get set up in Jira and stay on track in terms of documentation and task tracking. We are in the process of setting up dashboards in Jira to make it most usable and efficient for each of us stay in touch with all of our projects and responsibilities. 

One important point related to tasks in Jira is that when a person is assigned a task, that person is really being made responsible for completion of that task and is responsible for assigning others to sub-tasks as needed to get the work done. The fact that you are assigned a task does not mean that you are responsible for working on that task by yourself or in isolation from the group. All tasks can be broken up into smaller more manageable tasks (right-sized) so that they can be completed as quickly as possible and also assigned to others in the group without putting an undue time burden on the person assigned. 

### Use GitHub as Our Code Repository

It was decided that we would bring our GitHub repository in house and run it on our own servers. The cost is reasonable - only about double the $1200 per year that we pay now for hosted GitHub. We plan to explore all of the functionality of GitHub within our own environment (Git pages and documents -- written in MarkDown -- and  the GitHub API that handles issue and commit tracking, as well as wikis). At the same time, we have to make sure that our enterprise GitHub server is accessible for our external consultants and that they are able to interact seamlessly with it. 

### Use a Mongo (or other Document) Database and SQL Server

Mongo represents a significant change in the way that we store data; it is also likely to have significant repercussions for how we manage our databases and even how we organize the data to deliver an application. There was a good deal of discussion by the group about Mongo being very different than SQL and that in some cases, Mongo may be a poor fit. There was also quite a bit of uncertainty about the maintenance and management requirements of moving to Mongo on a large scale. Our conclusion is that at this time, Mongo is very much a learning process for all of us -- developers, database administrators, and infrastructure folks. Starting this transition with smaller applications rather than our largest, most complex apps is recommended. The move of the Hub to Mongo, in particular, is very much in the trial, prototyping stage and needs quite a bit more careful attention in order to understand its effects on our existing processes. 

Additionally, in the process of evaluating Mongo, we don't want to close off looking at alternative document databases, particularly those that may offer benefits from a query language, deployment and management or data replication perspective. While we are excited about Mongo and plan to all get trained on developing and maintaining it, we also will remain open to potentially superior document Db platforms (or alternatives with lower barriers to entry that might provide a simple bridge between the relational and document database worlds. 

### Use Node and relevant JS libraries as a platform for backend