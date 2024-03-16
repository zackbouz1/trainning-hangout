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
