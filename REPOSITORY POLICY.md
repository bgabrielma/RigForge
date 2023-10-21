### Repository Schema![repository_schema](https://github.com/bgabrielma/RigForge/assets/25841296/e3a9d1e6-b47c-42ed-9d56-0a11d0e7d7f2)
# Branches Meaning
## Production
The `production` branch in our GitHub repository holds our main, stable codebase. Code in this branch is thoroughly tested and represents the latest stable release. All merges to `production` should be made with care, ensuring only robust, production-ready changes are included. This branch serves as the foundation for our live deployments.
## Staging
The `staging` branch in our GitHub repository is dedicated to reviewing and consolidating all development work. Before changes are moved to the production branch, they are first merged to `staging`. This ensures that new features, bug fixes, or updates are collectively tested in a near-production environment, helping to catch potential issues before they reach the live version.
## Development
The `development` branch in our GitHub repository serves as the primary workspace for addressing and resolving all tasks assigned for the upcoming release. As new features, fixes, and updates are worked upon, they are merged into this branch. Once tasks are completed and tested, the `development` branch's contents are then promoted to more advanced stages, like `staging` or `production`, in our release cycle.
## Sub-branch Naming Policy for the `development` Branch
When creating sub-branches for the `development` branch, we employ a systematic naming approach to ensure clarity and traceability. Each sub-branch is named based on the reference number of its corresponding Trello card, followed by a brief title that offers a snapshot of its purpose. The format used is `#<Trello-Card-Number>-short-title`. For instance, a sub-branch addressing card #1 with a feature related to user authentication might be named `#1-user-auth`. This naming convention aids in swiftly associating branches with their Trello tasks and understanding their primary focus at a glance.
![trello_card_example](https://github.com/bgabrielma/RigForge/assets/25841296/153e0139-84ac-4cf4-811d-ec0205f754fa)
## Branch merge system
Once a task within a sub-branch is completed, it's imperative to initiate a Pull Request (PR) for that specific task. This PR serves as a gateway for the team to review, comment on, and eventually approve the changes, ensuring that our code maintains its quality and consistency before being merged into the main `development` branch.
It's worth noting that direct pushes to the `staging` and `production` branches are strictly prohibited. All code must first pass through the review processes and be merged appropriately to maintain the integrity of our staging and production environments.
