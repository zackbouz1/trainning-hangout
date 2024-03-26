# Github Foundations Practice Questions

## GitHub Projects
#### p001. (a very popular exam question) GitHub built-in Project Workflows allows you to automate what happens based on specific events. what are the Built-in Workflows? (list 8)
  - [ ] Item Labeled (don't fall for this)
  - [x] Item added to project
  - [x] Item reopened 
  - [x] Item closed
  - [x] Code changes requested
  - [x] Code review approved
  - [x] Pull request merged
  - [x] Auto-archive items
      * filters: is:issue is:closed updated:<@today-2w    --note: Using the updated operator means that your workflow will run every 12 hours
      * Action: Archive Item
  - [x] Auto-add to project
      * filters: is:issue,pr is:open label:bug
      * Action: Add the item to the project

#### p002. Which GitHub built-in Project Workflows are turned on by default when you create a new project? (choose 2)
  - [ ] Item added to project
  - [ ] Item reopened 
  - [x] Item closed
  - [ ] Code changes requested
  - [ ] Code review approved
  - [x] Pull request merged

#### p003. Project Insights lets you create charts about GetHub Project. List the chart types available under Project Insight? (choose 2)
  - [x] Current Charts: Track bugs opened and closed each iteration (X = Iteration#  , Y = number of items by status , Legend = Status)
  - [x] Historical Charts: track changes to the state of your project items over time (e.g., the X axis is always time)
  - [ ] User Chart
  - [ ] Team Chart

#### p004. what is the maximum number of items that can be included and displayed in a GitHub Project
  - [ ] 100
  - [ ] 600
  - [x] 1200
  - [ ] 2000

#### p005.Jerry is managing a very large project and he is worried the number of items in the GitHub Project will soon reach the 1200 items limit. What Should Jerry do?
  - [ ] Call GitHub premium support and request and request a quota increase
  - [x] Turn on the Project's Auto-archive items workflow to auto-archive completed items after 2 weeks
  - [ ] Switch to the paid plan
  - [ ] Delete the closed issues so they don't appear in the project

## GitHub Issues
#### z101.In a free GitHub plan, what is the maximum number of people that can be assigned to an issue or PR in a public repository and in a private repository?
  - [ ] Under the GitHub's free plan, you can assign limited number of assigneds to an issue or PR in a Public repo and up to 10 assignees in a private repo
  - [x] Issues and pull requests in public repositories, and in private repositories for a paid account, can have up to 10 people assigned. Private repositories on the free plan are limited to one person per issue or pull request.
  - [ ] Under the GitHub's free plan, you can assign up to 100 assigneds to an issue or PR for a Public repo and up to 10 assignee for a private repo
  - [ ] There is no limit on the number of assignees in the GitHub's free plan

#### z102. Who can assign Issues and PRs to other GitHubs users?
  - [ ] Only the repository owner can assign Issues and PRs
  - [x] Anyone with write access to a repository can assign issues and pull requests.
  - [ ] Only Contributors and Owners
  - [ ] Anyone with access to the repository can assign Issues and PRs

## GitHub Security Capabilities( DevSecOps)
**Important Exam Notes:** 
 - GitHub Advanced Security Features for users are available for public repositories for free.
 - Organizations using GitHub Enterprise Cloud with a **license for GitHub Advanced Security** can also enable Advanced Security Features for users on their private and internal repositories.

### Supply Chain
 - *Dependency Graph:* view your dependencies
   - *Advisory database:* canoncial database of dependency vulnerabilities
   - *Security alerts and updates:* notifications for vulnerabilities in your dependencies, and pull requests to fix them
 - *OSS Vulnerability Scanning:*
     - Dependabot: Dependabot alerts are free to use for all repositories on GitHub.com. Advanced capabilities, like the ability to create **custom auto-triage rules** for Dependabot alerts, are available (for free) on public repositories only or Organizations with Advanced Sercurity license.


### Code
 - *Secret Scanning Alerts (Advanced security):* Find API tokens or other secrets exposed anywhere in your git history
     - Custom Regex
     - Private-Secret-Scanning
     - Public-Secret-Scanning
 - *CodeQL Scanning (Advanced security):* Static analysis of every git push, integrated into the developer workflow.

### Development Lifecycle 
 - *Branch protection rules:* Enforce requirement for pushing to a branch and merging PRs
   - Advanced Security feature: Branch protection rule can require the code to pass a series of Status Checks before allowing the PR - e.g., Code should pass CodeQL analysis, Python code should be properly formatted.
 - *Commit signing:* Enforce requirement that all commits are signed

## GitHub Organization and Repository Roles
#### s201. what are the available access permissions in GitHubs Personal Accounts? (Choose 2)
  - [x] Repository Owner has full control of the repository and its configurations and can invite collaborators.
  - [ ] Repository Reader can read contents but cannot do anything else (incorrect, there is no READER role in Presonal account)
  - [x] Repository Collaborators can pull (read) the contents of the repository and push (write) changes to the repository
  - [ ] Repository Maintainners can open/close/reopen issues and PRs (incorrect, there is no MAINTAINNER role in Personal Accounts)

## Advanced Git Operations
#### 107. After making some major changes to your code, you are a little nervous about committing. What command would you use to review the commit prior to making it?
  - [ ] git commit --verify
  - [ ] git notes show
  - [ ] git commit preview
  - [x] git commit --dry-run
    
#### 108. What statement best describes Git's concept of HEAD?
  - [ ] a pointer to the most recently changed file in the stage/index
  - [ ] a pointer to the master branch
  - [x] a pointer to the most recent commit in the currently checked-out branch
  - [ ] a pointer to where the repository is stored in memory

#### 109. After staging changes to several files, you realize the changes to the config.properties file are incorrect, and need to be removed from the stage and working directory. What command can you use to remove the staged changes to the file?
  - [x] git reset HEAD^ -- config.properties
  - [ ] git rm config.properties
  - [ ] git rf config.properties
  - [ ] git checkout HEAD -- config.properties
    
#### 110. After a recent release, an issue is created that indicates a problem with a newly added configuration property named MaxConnections. What command can find all commits that add or remove the string MaxConnections?
  - [ ] git grep -a "MaxConnections"
  - [ ]  git log --search-string "MaxConnections"
  - [x]  git log -S "MaxConnections"
  - [ ]  git commit --with "MaxConnections"
    
#### 111. Your company has moved its remote repository to GitHub at this location: https://github.com/yourcompany/core-api.git. What command updates the remote repository, named origin, to point to the new remote repository at this location?
  - [ ] git remote create-update origin https://github.com/yourcompany/core-api.git
  - [ ] git remote update origin https://github.com/yourcompany/core-api.git
  - [x] git remote set-url origin https://github.com/yourcompany/core-api.git
  - [ ] git remote add https://github.com/yourcompany/core-api.git
    
#### 112. When is the cherry-pick command used?
  - [x] when a commit from one branch needs to be copied into another branch
  - [ ] when the HEAD needs to be reset to a specific commit
  - [ ] when a specific commit needs to be pulled down from the remote repository
  - [ ] when a hook script needs to be invoked

#### 116. What would happen if you ran the git reset testfile.js command?
  - [ ] testfile.js would be reverted to a blank file.
  - [ ] testfile.js would be reset to its first saved state.
  - [x] testfile.js would be reverted to its last saved copy.
  - [ ] testfile.js would be removed from the stage/index area, if present.

## MANAGING MERGE
#### 118. When Git workflows contain a topic branch, what purpose does the topic branch serve?
  - [ ] Topic branches store unstable code until it is peer reviewed for integration into another feature branch.
  - [ ] Topic branches correspond to different stages of development and are always open for long-running branches to be pulled into.
  - [ ] Topic branches are used in waterfall development methodologies to track the state of the code during the various stages of waterfall.
  - [x] Topic branches are short-lived branches used to store work related to a particular feature.

#### 119. What practice can help reduce the chances of encountering a merge conflict?

  - [ ] Provide detailed commit messages that describe the changes being introduced by the commit.
  - [ ] make large commits that introduce multiple features.
  - [x] Keep local repository branches in sync with upstream branches in the remote repository by committing,pushing and pulling frequently.
  - [ ] Avoid frequent interaction with the remote repository to reduce the probability of pulling conflicts.
         
#### 120. What command can you use to remove untracked files from the working directory?

  - [ ] git rm -all
  - [ ] git rm --cached
  - [x] git clean -d -f
  - [ ] git checkout
