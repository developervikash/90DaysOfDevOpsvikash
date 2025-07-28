 Git Branching Strategy & Workflow



Updating a forked repository
When you fork a repository, you can make changes by:
1. Opening it via VS Code.
2. Creating a new branch.
3. Pushing the changes to your forked repository.

How many branches are there in Git?
Branching in Git
Everyone uses different branching strategies based on their project and codebase.However, commonly used branching strategies include:
MASTER/MAIN – STAGING – DEVELOPMENT – FEATURE

MASTER/MAIN Branch
* This branch contains live production code.
DEVELOPMENT Branch
* This branch contains the latest code changes that are being prepared for production.
FEATURE Branch
* Developers create feature branches from the development branch to work on a new feature.
* After completing the feature, it is merged back into the development branch.
STAGING Branch
* When the development branch is ready, its code is merged into staging.
* Testers test the staging branch.
* Once testing is successful, staging is merged into main/master.

Happy Scenario
All the above steps (feature → development → staging → master) are considered a happy scenario.

HOTFIX
* If an error occurs in production, a new branch is created directly from main/master called HOTFIX.
* After fixing the issue, the HOTFIX branch is merged back into main/master, and then staging & development branches are updated (pulled) to keep them in sync.

Definition:
A HOTFIX is a critical issue that appears in production and must be fixed immediately without going through the normal development process.

 Also there 

 if want to clone
 so it is called 

 Github to Github is called => Fork
 Github to Local us called => Clone