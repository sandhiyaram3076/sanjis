Developers create separate branches for independently working on features so that changes from other developers don't interfere with an individual's line of work. Developers can easily pull changes from different branches and also merge their code with the main branch. This allows easier collaboration for developers working on one codebase.

A branching strategy is a strategy that software development teams adopt for writing, merging and deploying code with the help of a version control system like Git.

Gitflow Workflow
GitFlow enables parallel development, where developers can work separately on feature branches, where a feature branch is created from a master branch. After completion of changes, the feature branch is merged with the master branch.

The types of branches that can be present in GitFlow are:

Master - Used for product release
Develop - Used for ongoing development
Feature Branching - branches off the develop branch to develop new features.
Release - Assist in preparing a new production release and bug fixing, typically branched from the develop branch, and necessitating merges back into both develop and master branches.
Hotfix - Hotfix branches aid in addressing discovered bugs swiftly, allowing developers to continue their work on the develop branch while the issue is resolved. Unlike release branches, hotfix branches are created from master branch specifically for critical bug resolution in the production release.

GitHub Flow
GitHub flow is a simpler alternative to GitFlow, idea for smaller teams. GitHub flow only has feature branches that stem directly from the master branch and are merged back to master after completing changes. They don't have release branches. The fundamental concept of this model revolves around maintaining the master code in a consistently deployable condition, thereby enabling the seamless implementation of faster release cycles, continuous integration and continuous delivery workflows.

The types of branches that can be present in GitFlow are:

Master - The GitHub Flow workflow initiates with the master branch, housing the most recent stable code prepared for release.
Feature - Developers initiate feature branches from the main branch to implement new features or address bugs. Upon completion, the feature branch is merged back into the main branch. If a merge conflict arises, developers are required to resolve it prior to finalizing the merge.

GitLab Flow
GitLab flow is also an alternative to GitFlow, designed to be more robust and scalable than GitHub Flow. Designed for teams using GitLab, a web-based Git repository manager, this approach streamlines development by concentrating on a solitary, protected branch, usually the master branch. Continuous integration and automated testing form the core elements of GitLab Flow, guaranteeing the stability of the master branch.

The types of branches that can be present in GitFlow are:

Master: Main production branch housing stable release ready code.
Develop: Contains new features and bug fixes.
Feature: Developers initiate feature branches from the develop branch to implement new features or address bugs. Upon completion, they integrate the changes from the feature branch into the develop branch.
Release: Prior to a new release, a release branch is branched off from the develop branch. This release branch serves as a staging area for integrating new features and bug fixes intended for the upcoming release. Upon completion, developers merge the changes from the release branch into both the develop and main branches.


Trunk Based Development
It is a branching strategy where developers work on a single "trunk" branch, mostly the master branch and use feature flags to isolate features until they are ready for release. This main branch should be ready for release any time. No additional branches are created. The main idea behind this strategy is to make smaller changes more frequently to avoid merge conflicts and the goal is to limit long-lasting branches. This strategy enables continuous integration and delivery, making it an attractive choice for teams aiming to release updates swiftly and frequently. It is particularly well-suited for smaller projects or teams seeking a streamlined workflow.

Source link: https://www.geeksforgeeks.org/git/branching-strategies-in-git/
