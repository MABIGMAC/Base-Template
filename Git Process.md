# **List base features of github**

| Feature                 | Description                                                                                                                                                                    |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Repositories            | Storage spaces for projects where all the files, revision history, and metadata are kept.<br />Each project typically has its own repository.                                  |
| Readme.md               | A markdown file in the repository that provides an overview of the project.<br />It often includes installation instructions, usage examples, and contact information          |
| Branches                | Separate lines of development within a repository.<br />Branches allow multiple people to work on different features or fixes simultaneously                                   |
| Commits                 | Snapshots of changes made to the repository.<br />Each commit includes a commit message explaining what changes were made and why                                              |
| Pull Requests           | Proposals to merge changes from one branch into another.<br />Pull requests facilitate code review, discussion, and quality control before integrating new code                |
| Issues                  | Tracking tools for bugs, tasks, and enhancements.<br />Users can open, discuss, and close issues to manage and organize work on the project                                    |
| Discussions             | Forums within a repository for community conversations.<br />Discussions can be used for brainstorming, Q&A, and general topic discussions                                     |
| Wikis                   | Collaborative documentation spaces within a repository.<br />Wikis are used to provide detailed information and documentation about the project                                |
| Projects                | Kanban-style boards for project management.<br />Projects can be used to organize and track progress on tasks, issues, and pull requests                                       |
| Milestones              | Grouping issues and pull requests into significant points in the project’s timeline.<br />Milestones help track progress towards large goals or releases                      |
| Git Workflows           | Prescribed methods for using Git and GitHub together to manage and streamline development processes                                                                            |
| Dependabot              | Automated tool that checks dependencies for vulnerabilities and suggests updates.<br />Dependabot helps keep projects secure by managing dependency updates                    |
| Branch Protection Rules | Settings that enforce certain workflows or approvals before a branch can be merged.<br />These rules help maintain the integrity of the main codebase                          |
| Git Pre-Commits         | Scripts that run automatically before a commit is finalized.<br />Pre-commit hooks can enforce code standards, run tests, or perform other checks                              |
| Github Pages and Wiki   | GitHub Pages allows users to host static websites directly from their repositories.<br />Wikis provide a collaborative space for project documentation and information sharing |

# STARLAB Augments

| Feature          | Augments                                                       |
| ---------------- | -------------------------------------------------------------- |
| Issues           | Template for Bugs/Features/Epics                               |
|                  | Additional Labels: Backend, Middleend, Frontend, Epic, feature |
| Pull Requests    | Template for Pull Requests                                     |
| Pre-Commit Hooks | Enforce Git conventions (feat, fix, docs, chores, etc.)        |
| Branches         | Release & Dev                                                  |
| Release          | Automated Release Manager (requires PR w Git Conventions)      |
| Monitoring       | Telegram Notif: Issues, PRs, Git Commits                       |
| Git Projects     | Data fields: Status, Priority, Size, Sprint (2 Weeks)          |
|                  | Epics Column                                                   |
|                  | Automated Roll over issues to next sprint                      |

# Git Process (Things Users need to memorise)

## Creating a new Epic issue

1. Via Project Board
   * Click "Add Item" under desired column
   * Enter name to create Draft
   * Click into it and "Convert to issue", selecting repo
   * Edit Description, enter /templates > epic
   * List the features(tasks) in the Epic
   * Fill in details and Assign labels
2. Via Issues Board
   * Creating a new issue, use Epic template
   * List the features(tasks) in the Epic
   * Add the sprint
   * Link to project and assign to Epic Column

## Creating a new feature issue

1. Via Project Board

   * Click "Add Item" under desired column
   * Enter name to create Draft
   * Click inside the new issue,
     * Edit and add /template for the feature template
     * Add the labels
     * Add the sprint
2. Via Issues Board

   1. Convert to Issue
      * Inside Epic issue, in the task list, click on the task
      * Click inside the new issue,
        * Edit and add /template for the feature template
        * Add the labels
        * Add the sprint
        * Link to project and assign to Todo Column
   2. Create new Issue
      * Add new feature template
      * Adjust the labels
      * Add the sprint
      * Goto the Epic issue and edit, adding the index of the new feature issue into the task list

## Creating a new bug issue

1. Via Project Board
   * Click "Add Item" under desired column
   * Enter name to create Draft
   * Click into it and "Convert to issue", selecting repo
   * Edit Description, enter /templates > Bug
   * Fill in details and Assign labels
2. Via Issue Board
   1. Create new issue
   2. Add new bug template
   3. Adjust the labels
   4. Add the sprint

## Creating Research Tickets

1. Via Project Board

   * Click "Add Item" under desired column
   * Enter name to create Draft

## Branching off and coding

1. All dev work should be branched from the dev branch and PR'd into it when completed
2. New Branches must have the prefix of **git conventions**, followed by **/** (e.g. feat/Title)
3. Git commits must follow git convention format (Enforced by STARLAB Augments: Pre-commit hooks)
4. All Pull requests **must** follow git convention format in the title naming
   1. Setting fix: or feat: will help the automated release manager identify those pull requests to be included into the changelog

## Release

1. Create a PR from dev to release
2. A PR will be automated to create a new Tagging

# Sprints

## How to create a new sprint

* Its autocreated from the "iteration" data field,
  1. goto settings
  2. goto the iteration section
  3. Add iteration

## Adding a new item to Sprint

* Add a feature, link to the project

## Rolling over an item to the next sprint

* Its automated to rollover to the next sprint as long as the issue is in the columns (Todo, in progress, in review or Epic)

## Remove an item from sprint

* Go to the issue and untag the iteration

Added feature1