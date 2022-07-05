# WORKING WITH JIRA

For software projects, there are three main sections to consider when working with Jira, namely: Planning, Development, and Operations. 
The Planning section(which is the most important section) is subdivided into various useful components as well, the most prominent ones being Roadmap, Backlog, Active Sprints, Issues. 
Under Development, we have mostly the list of repositories that we will be working with for the project. 
The operations involves the CI/CD tools and services required for the project.

## PLANNING

1. **Roadmap:** This is basically as the name implies is a strategic tool that can help graphically illustrate both long-term and short-term plans. In short, it says where you are and where you plan on going within the next few months/years on a particular project. It is mainly divided into epics, stories, and tasks.
  - **Epics** are large bodies of work that can be broken down into a number of smaller tasks (called stories).
  - **Stories** are the small, lightweight requirements of the project broken down from the epics.
  - **Tasks** are actual implementation of the stories.

2. **Backlog:** According to google, in Agile development, a product backlog is a prioritized list of deliverables (such as new features) that should be implemented as part of a project or product development. It's a decision-making artifact that helps you estimate, refine, and prioritize everything you might sometime in the future want to complete. This is exactly what this module does on the Jira application. It helps you visualize, analyse and gives you a general insight on project performance, speed, trajectory, and efficiency. 

3. **Active Sprints:** the Active sprints of a Scrum board displays the issues that your team is currently working on. You can create and update issues, and drag and drop issues to transition them through a workflow. The workflows in this case include: To Do, In-Progress, Code-Review, Validation, and Done.
  - **To Do** are tasks that have not yet commenced, they can be assigned or unassigned to an engineer.
  - **In Progress** are tasks that have already been assigned to an engineer and corresponding actions have commenced.
  - **Validation** are tasks that have been completed by an engineer and awaiting peer review/validation.
  - **Done** are completed tasks that have been validated and approved by the appropriate entity(ies).

4. **Issues** are every task, story and epic.  


## DEVELOPMENT

1. **Code:** This consists of all the various repositories that contain project files, assets, resource materials, learning materials, articles, documentation etc. 

2. **Releases:** This is where all app releases and their variants appear.

## OPERATIONS
1. **Deployments**  This mainly consist of the Continuos deployment and Integration tools, services, resources that

1. We use `Engineering` board on Trello for all of our engineering activities. If you're not on this board. Let your manager know.
1. Repositories are labels in Trello. For ex: We have a label on `Engineering` board for cloudboost/cloudboost project, cloudboost/user-service, etc.
1. We've created many list on the  `Engineering` board:
  - **Ideas:** These are tasks or cards which are ideas or feature requests from our customers that *may or may not be* implemented.
  - **Unassigned:** These are tasks or cards not assigned to anyone.
  - **To-Do:** When the card is assigned to someone. It's usually in To-Do.
  - **Doing:** Move the card here when you're working on it. Only one card assigned to you should be in doing. Write code + tests before moving the card to `Code Review`
  - **Code Review:** Assign the card to your code-reviewer for review.
  - **Deployed to Staging:** When the feature is deployed to staging and is assigned to Quality Assurance team.
  - **Quality Assurance:** Quality check for the task.
  - **Deploy to Production Pending:** Card assigned to Ops and deploy to production is pending.
  - **Deployed to Production:** When a task is on production.
1. When a card is assigned to you. You'll get a notification and It should be on the To-Do list.
1. *Tip:* If the board has a lot of cards and is messy. You can only see cards assigned to you or by label by Filter Card feature in the Trello more menu. This saves a lot of time looking up cards assigned to you.
1. **Important:**
  - When you've been told a task by your manager verbally. Add a card immediately to To-Do, describe a task and assign that card to yourself.
  - Never work on more than one card. ONLY one card assigned to you should be in the `Doing` list.
  - Only push card to `Done` when you're done with the feature / task, done with writing tests, and also have manually tested the feature. Push the card to `Code Review` when you're done and ping your code reviewer for review. Assign the card to him.
  - If there are any reviews in the `Code Review` stage, the card will be pushed to `Doing` list by your reviewer. The card will be re-assigned to you.
  - Once you're done with all the code reviews. The task will be deployed to staging and will be assigned to `Quality Assurance` team for final check. If there are any bugs found here. It'll be pushed to `Doing` and will be re-assigned to you.
  - Your task is ONLY done with it has passed `Quality Assurance`, and is in the `Deploy to Production Pending` list. In this case, the card will be assigned to dev-ops team and they will take care of shipping the feature in production.
  - If you're in the dev team and your card gets moved back and forth between `Quality Assurance` and `Doing`. that's a bad sign and affects very negatively on you. Continue to do this, and you'll not be working with us.  It's your job to make sure the task is without any bugs before you pass that to `QA` team.
