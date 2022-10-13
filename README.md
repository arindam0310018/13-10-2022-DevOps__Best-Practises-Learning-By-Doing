# AZURE DEVOPS BEST PRACTISES: LEARNING BY DOING

Greetings my fellow Technology Advocates and Specialists.

In this Session, I will provide you real-time insights on __AZURE DEVOPS BEST PRACTISES: LEARNING BY DOING__. 


| __IMPORTANT TO NOTE:-__ |
| --------- |
| For Ease of Explanation, I will provide Best Practises details for Azure Devops: __REPOSITORIES__, __PIPELINES__, __BOARDS__ & __WIKI__ |


| __BEST PRACTISES FOR REPOSITORIES:-__ |
| --------- |
| __Proper Folder Structure__ per Repository. |
| __Repository Security__, if we have multiple Repositories under same DevOps Project. |
| __Branching Strategy:__ 1) Feature to Development Branch, 2) Development to Main Branch. |
| Clean Commit History with Human Readable comments per commit. |
| Build Validation for Main Branch. |
| __Pull Request (PR)__ must have an Approval in Place to review the changes (Part of Code Review). |


| __HOW BRANCHING STRATEGY WORKS:-__ |
| --------- | 
| 1. Per Developer(s) – Working on Feature Branch. |
| 2. All Developer(s) Changes in Feature Branch are then Merged into Development Branch by Squash Commit using Pull Request (PR). | 
| 3. Feature Branch __DELETED__ post Squash Commit to Development Branch. | 
| 4. All changes committed in Development Branch is then pushed to MAIN Branch by Squash Commit using a Single Pull Request (PR). |
| 5. Development Branch __REMAINS__ post Squash Commit to MAIN Branch. |
| 6. Development and MAIN Branch should be in complete Sync (0 Commits Behind). |


| __BEST PRACTISES FOR PIPELINES:-__ |
| --------- |
| 1. YAML Based pipeline over Classic as it can be Version controlled. |
| 2. Reusable Templates. |
| 3. Proper Folder Structure for Each Pipeline. |
| 4. Proper Naming Convention for Each Pipeline. |
| 5. Pipeline Name and Folder should have a relevance with the Code Repository. |
| 6. Setup Pipeline Environment(s), Attach Approval Gate and Associate Pipeline(s) appropriately per Environment. |
| 7. Avoid using Pipeline Local Variable Groups or Variable Groups associated with Key Vault. All Key value pair needs to stored in Key Vault and should be retrieved as Pipeline Task. |
| 8. Use of Azure DevOps Marketplace Extensions. |


| __BEST PRACTISES FOR BOARDS:-__ |
| --------- |
| 1. If a Single DevOps Project is used to host Multiple Application Projects, then there should be __distinct Boards Per Application Project to manage Backlogs and Sprints__. |
| 2. __Permissions__ should be set accordingly for Single/Multiple Board(s) preferably using __AAD Groups__. |
| 3. __Pull Request (PR) should be linked with Work items__ in DevOps Boards so that when Pull Request (PR) is approved, it closes the Work item at the same time. This automatically puts a comment with the link to commit against the linked work item. |


| __BEST PRACTISES FOR WIKI:-__ |
| --------- |
| 1. __Create Wiki as Repo__ to version control. |
| 2. __Use Mermaid Diagrams__ below – a) Flow Chart b) Gantt Chart c) Sequence Diagram |


__Hope You Enjoyed the Session!!!__

__Stay Safe | Keep Learning | Spread Knowledge__
