## GitHub Projects
z001. (very likely exam question) GitHub built-in Project Workflows allows you to automate what happens based on specific events. List the Built-in Workflows?
  - [x] Item added to project
  - [x] Item reopened 
  - [x] Item closed
  - [x] Code changes requested
  - [x] Code review approved
  - [x] Pull request merged
  - [x] Auto-archive items
        -- filters: is:issue is:closed updated:<@today-2w    --note: Using the updated operator means that your workflow will run every 12 hours
        -- Action: Archive Item
  - [x] Auto-add to project
        -- filters: is:issue,pr is:open label:bug
        -- Action: Add the item to the project

z002. Which GitHub built-in Project Workflows are turned on by default when you crate a new project? (choose 2)
  - [ ] Item added to project
  - [ ] Item reopened 
  - [x] Item closed
  - [ ] Code changes requested
  - [ ] Code review approved
  - [x] Pull request merged


## Git Commands
107. After making some major changes to your code, you are a little nervous about committing. What command would you use to review the commit prior to making it?
     - [ ] git commit --verify
     - [ ] git notes show
     - [ ] git commit preview
     - [ ] git commit --dry-run
    
108. What statement best describes Git's concept of HEAD?
     - [ ] a pointer to the most recently changed file in the stage/index
     - [ ] a pointer to the master branch
     - [ ] a pointer to the most recent commit in the currently checked-out branch
     - [ ] a pointer to where the repository is stored in memory

109. After staging changes to several files, you realize the changes to the config.properties file are incorrect, and need to be removed from the stage and working directory. What command can you use to remove the staged changes to the file?
     - [ ] git reset HEAD^ -- config.properties
     - [ ] git rm config.properties
     - [ ] git rf config.properties
     - [ ] git checkout HEAD -- config.properties
    
110. After a recent release with a stack trace, an issue is create that indicates the problem is with a newly added configuration property named MaxConnections. What command can find all commits that add or remove the string MaxConnections?
     - [ ] git grep -a "MaxConnections"
     - [ ]  git log --search-string "MaxConnections"
     - [ ]  git log -S "MaxConnections"
     - [ ]  git commit --with "MaxConnections"
    
111. Your company has moved its remote repository to GitHub at this location: https://github.com/yourcompany/core-api.git. What command updates the remote repository, named origin, to point to the new remote repository at this location?
     - [ ] git remote create-update origin https://github.com/yourcompany/core-api.git
     - [ ] git remote update origin https://github.com/yourcompany/core-api.git
     - [ ] git remote set-url origin https://github.com/yourcompany/core-api.git
     - [ ] git remote add https://github.com/yourcompany/core-api.git
    
112. When is the cherry-pick command used?
     - [ ] when a commit from one branch needs to be copied into another branch
     - [ ] when the HEAD needs to be reset to a specific commit
     - [ ] when a specific commit needs to be pulled down from the remote repository
     - [ ] when a hook script needs to be invoked

116. What would happen if you ran the git reset testfile.js command?
     - [ ] testfile.js would be reverted to a blank file.
     - [ ] testfile.js would be reset to its first saved state.
     - [ ] testfile.js would be reverted to its last saved copy.
     - [ ] testfile.js would be removed from the stage/index area, if present.

## MANAGING MERGE
118. When Git workflows contain a topic branch, what purpose does the topic branch serve?
     - [ ] Topic branches store unstable code until it is peer reviewed for integration into another feature branch.
     - [ ] Topic branches correspond to different stages of development and are always open for long-running branches to be pulled into.
     - [ ] Topic branches are used in waterfall development methodologies to track the state of the code during the various stages of waterfall.
     - [ ] Topic branches are short-lived branches used to store work related to a particular feature.

119. What practice can help reduce the chances of encountering a merge conflict?

     - [ ] Provide detailed commit messages that describe the changes being introduced by the commit.
     - [ ] make large commits that introduce multiple features.
     - [x] Keep local repository branches in sync with upstream branches in the remote repository by committing,pushing and pulling frequently.
     - [ ] Avoid frequent interaction with the remote repository to reduce the probability of pulling conflicts.
         

