# Github Foundations Practice Questions
Credit goes to:

   - [Exam Pro's free GitHub Foundations training](https://www.exampro.co/github-foundations)
   - [FREE GITHUB FOUNDATIONS PRACTICE TEST](https://ghcertified.com/practice_tests/foundations/)
   - [GitHub Docs](https://docs.github.com/en)

## Copilot (this is accurate as of Q1 2024 - but things are quickly changing)
 - GitHub Copilot is an AI-powered that offers code autocomplete-style suggestions as you code.
 - To use GitHub Copilot, sign up for Copilot via its web page, and then install it as an extension into your IDE. Extensions are available for major IDEs like Visual Studio and Visual Studio Code.
 
### Plans (as of Q1 2024)
  - Copilot Individual is free for verified students, teachers, and maintainers of populare open-source projects
  - Copilot Business: requires a paid subscription. It offers an Orangization-wide policy management feature and AUdit Logs
  - Copilot Enterprise plan is  available for enterprises that use GitHub Enterprise Cloud. The plan Offers all the functions available in Copilot Business, PLUS a  the ability to chat with Copilot in the browser in github.com


#### c001. You are the GitHub administrator in an organization. Your manager is investigating the use of Copilot to speed up code delivery but is concerned about security. She wants to implement a company-wide security policy and exculde certain file types from being evaluated. Which Copilot plan should you choose to meet your manager's requirements?
  - [x] [Copilot Business](https://docs.github.com/en/copilot/copilot-business/about-github-copilot-business)
  - [x] Copilot Enterprise
  - [ ] Copilot Individuals

#### c002. How does GItHub Copilot recognize prompts for generating code suggenstion in a supported IDE? (Choose 2)
  - [x] [You can describe something you want to do using natural language within a **comment** in one of the supported file extensions (e.g., .py or .js), and GitHub Copilot will suggest the code to accomplish your goal.](https://docs.github.com/en/enterprise-cloud@latest/copilot/using-github-copilot/getting-started-with-github-copilot#generating-code-suggestions-from-comments-2)
  - [x] using one of the supported languages, type a meaningful function header (e.g., function calculateDaysBetweenDates(begin, end)). GitHub Copilot will automatically suggest an entire function body in grayed text.
  - [ ] Using a search function

#### c003. how do you accept a suggestion from GitHub Copilot in a supported file extension (e.g., .JS or .PY)?
  - [x] [by Pressing the "Tab" key](https://docs.github.com/en/enterprise-cloud@latest/copilot/using-github-copilot/getting-started-with-github-copilot#seeing-your-first-suggestion-2)
  - [ ] by pressing the "Enter" key
  - [ ] By pressing "Ctrl-A" combination

#### c004. what are the use cases for [GitHub Copilot Chat?](https://docs.github.com/en/copilot/github-copilot-chat/about-github-copilot-chat#use-cases-for-github-copilot-chat)
  - [x] Generating Unit test cases
  - [x] Explaining code and suggesting improvements
  - [x] Proposing code fixes
  - [X] Answering coding quesitons 

## Gists
**Exam Notes:**
  - Public gists show up in Discover, where people can browse new gists as they're created.
  - Secret gists don't show up in Discover and are not searchable unless you are logged in and are the author of the secret gist.
    - Secret gists aren't private. If you send the URL of a secret gist to a friend, they'll be able to see it.
  - you can clone a gist and make commits the same as you would with any Git repository.

#### G100. Can you change a gist from public to secret after creating it?
  - [ ] Yes
  - [x] No: After creating a gist, you cannot convert it from public to secret.. However, a secret gist can be made public by editing the gist and updating the visibility to public. 

## GitHub Projects
#### p001. (a very popular exam question) GitHub built-in Project Workflows allows you to automate what happens based on specific events. what are the Built-in Workflows? (Select 8)
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

#### p006. What are the different available options for adding issues and pull requests to a GitHub Project board?
  - [ ] Only automatically using project workflows
  - [x] individually, automatically, or in bulk
  - [ ] Only individually or in bulk
  - [ ] only manually

#### p007. List the types of project that GitHub support
  - [ ] Peraonal Project
  - [ ] Team project
  - [x] Organization project: this is only available within an organization. To create, click Profile Picture => Your Organization => Projects => New Projects
  - [x] User Project: available to personal account. To create, click profile Picture => Your Projects => New Project


## GitHub Issues and Pull Requests
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

#### z103. [How can you use the advanced search feature to find all pull requests that contain comments that mention the word "style" and mention you?](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-a-user-thats-involved-in-an-issue-or-pull-request)
  - [ ] use the query;   is: pr is:closed
  - [x] use the query:   style in:comments  is:pr invovlves:@me
  - [ ] use the query:   is:issue  assignee:@me
  - [ ] use the query:   is:pr commenter:@me	

## GitHub Security Capabilities( DevSecOps)
**Important Exam Notes:** 
 - GitHub Advanced Security Features for users are available for public repositories for free.
 - Organizations using GitHub Enterprise Cloud with a **license for GitHub Advanced Security** can also enable Advanced Security Features for users on their private and internal repositories.
 - Repository administrators and organization owners can configure repository security settings.

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

#### s201. What can you find in the security tab of a repository?
  - [ ] A list of all teh GitHub Issues that have been opened in the repository for security reasons
  - [ ] A list of all best practices that GitHub recommends for software security
  - [x] A Security Overview of that repository such as vulnerabilities in dependencies, code scanning results, and secret scanning findings
  - [ ] Contact information to teh security team at GitHub

#### s202. What is CodeQL?
  - [x] A code analysis tool
  - [ ] A text editor
  - [ ] A programming language
  - [ ] A version control system

#### s203. Which security feature is available to all GitHub repositories and does NOT require a GitHub Advanced Security (GHAS) License? (select 2)
  - [x] Depandabot Alters: track security vulnerabilities that apply to your repository's dependencies. This is included in all plans under: Repository => Secrutiy => Vulnerability Alerts. Depandabot Configurations are saved in file: /.github/dependabot.yml  
  - [x] Dependency graph: Included in all plans under: Repository => Insights => Dependency Graph
  - [ ] Secret Scanning
  - [ ] Dependency Review
  - [ ] Code Scanning (CodeQL)

## GitHub Organization and Repository Roles
**Exam Notes:**
  - You can define _CODEOWNERS_ in public repositories with GitHub Free and GitHub Free for organizations, and in public and private repositories with GitHub Pro, GitHub Team, GitHub Enterprise Cloud, and GitHub Enterprise Server.
  - To use a CODEOWNERS file, create a new file called CODEOWNERS in the .github/, root, or docs/ directory of the repository, **in the branch** where you'd like to add the code owners. If CODEOWNERS files exist in more than one of those locations, GitHub will search for them in that order and use the first one it finds.
  - [Roles in an Organization](https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization)

#### s211. what are the available access permissions in GitHubs Personal Accounts? (Select 2)
  - [x] Repository Owner has full control of the repository and its configurations and can invite collaborators.
  - [ ] Repository Reader can read contents but cannot do anything else (incorrect, there is no READER role in Presonal account)
  - [x] Repository Collaborators can pull (read) the contents of the repository and push (write) changes to the repository
  - [ ] Repository Maintainners can open/close/reopen issues and PRs (incorrect, there is no MAINTAINNER role in Personal Accounts)

#### s212. What are the possible GitHub account types? (Select 3)
  - [ ] Shared accounts
  - [x] Enterprise accounts: allow administrators to centrally manage policy and billing for multiple organizations and enable innersourcing between the organizations.
  - [ ] Company accounts
  - [x] Organization accounts: offer EMU, SAML, additional repository roles
  - [x] Personal accounts

#### s213. What is the purpose of a "CODEOWNERS" file?
  - [ ] The CODEOWNERS file contains contact details to the repository owners.
  - [ ] The CODEOWNERS file includes information about the code quality and the maintainability of the code.
  - [x] The CODEOWNERS file allows you to define individuals or teams that are responsible for specific areas of the codebases. Code owners are automatically requested for review when someone opens a pull request that modifies code that they own.
  - [ ] The CODEOWNERS file contains information about the software licensing fees and conditions under which the code can be used

#### s214. How can you enforce status checks passing before merging a pull request to the _main_ branch?
  - [ ] By running tests locally prior to pushing to the remote repository
  - [ ] By making the repository private
  - [x] [By creating a branch protection rule](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/about-protected-branches#about-branch-protection-settings)
  - [ ] By using GitHub Actions

#### s215. What are Enterprise Managed Users (EMU)?
  - [ ] It's a user account without access to GitHub web UI but is rather only used for automation tasks in your GitHub Enterprise
  - [x] It's a GitHub Enterprise feature that allows you to manage user access from an external identity provider such as Azure AD or Okta
  - [ ] It's a GitHub Enterprise support user that can be used to manage your Enterprise by GitHub Support once requested
  - [ ] It's a shared user account that can be used by multiple users in your Enterprise.


#### s216. Which of these is NOT a role in a GitHub Organization?
  - [ ] Outside Collaborator
  - [ ] GitHub App Manager: can manage the settings of some or all GitHub App registrations owned by the organization.
  - [x] Organization architect
  - [ ] Organization Owner
  - [ ] Organization moderator: allowed to block and unblock non-member contributors, set interaction limits, and hide comments in _public repositories_ owned by the organization. 
  - [ ] Security manager: permissions to view security alerts and manage settings for code security across your organization, as well as read permissions for all repositories in the organization.
  - [ ] Billing manager
  - [ ] Organization member: Organization members have a number of default permissions including the ability to create repositories and projects.

#### s217. What is the role of an organization security manager?
  - [ ] Security managers are organization members who can manage the billing settings for your organization, such as payment information. (incorrect, this is the role of the Billing Manager)
  - [ ] Security managers are organization members who have complete access to the organization. (Incorrect, this is the role of the Organization Owner)
  - [ ] Security managers are organization members who, in addition to their permissions as members, are allowed to block and unblock non-member contributors, set interaction limits, and hide comments in public repositories owned by the organization. (Incorrect, this is the role of the Organization Moderator)
  - [x] Security managers are organization members who can view security alerts and manage settings for code security across your organization, as well as read permissions for all repositories in the organization.

#### s218. While role can manage access to a repository in an organization?
  - [x] People with admin access to a repository can grant access to teams and people.
  - [ ] People with Security manager role can grant access to teams and individuals
  - [ ] People with Triage role can manage grant and remove members access

#### s219. Jenna is managing a popular repository in her organization with many teams and individuals access levels. She is concerned some individuals may have mixed roles access. How can she investigate?
  - [x] [Jenna should go to the repository access page and look for the warining message "Mixed Roles" displayed next to the individual account](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-teams-and-people-with-access-to-your-repository)
  - [ ] Jenna should go to the Repository Insight page and check if a member belongs to multiple teams
  - [ ] Jenna should monitor members activity and see if someone can perform additional operations than they should

#### s220. You are the maintainer of a popular open source project and you want to create a guideline for repository collaborators. What should you do?
  - [x] Create a CONTRIBUTING.md file which contains the guidelines and save it in your repository's root, docs, or .github directory.
  - [ ] Add the guideline to the ISSUE_TEMPLATE.md
  - [ ] Add the guideline to the CODEOWNERS file
  - [ ] Add the guideline to the READ.me file

## Codespace and github.dev 

#### d301. What is a GitHub Codespace?
  - [x] It is a preconfigured development environment specifically setup for a repository. It allows developers to immediately start writing code for a project without having to setup a local development environment.
  - [ ] It is an interactive coding environment that requires special hardware to use
  - [ ] It is an AI-Powered coding tool that auto-generate near flawless code
  - [ ] It is a user communitee for exchanging code.

#### d302. How can you customize the environment that is run in GitHub Codespaces?
  - [ ] By creating a custom DockerFile in the root of your repository
  - [ ] By creating a .github/codespaces.yml configuration file
  - [x] By creating a .devcontainer/devcontainer.json configuration file
  - [ ] By creating custom machine images with the repository installed

#### d303. What are the different possible lifecycle phases for a GitHub Codespace?
  - [ ] Create, Delete
  - [ ] Create, Stop, Delete
  - [ ] Create, Rebuild, Delete
  - [x] [Create, Rebuild, Stop, Delete](https://docs.github.com/en/codespaces/getting-started/understanding-the-codespace-lifecycle)

#### d304. If you stop your GitHub Codespace environment can you come back to the changes later if you haven't committed them?
  - [x] Yes, that's the default behavior when stopping and starting a GitHub Codespece.
  - [ ] No, these changes will be lost. You need to commit them before stopping the Codespace

#### d305. What is a GitHub Codespace deep link?
  - [x] [a hyperlink to take people straight to a page for creating a codespace, with your choice of options preconfigured. Alternatively you can link to the "Resume codespace" page.](https://docs.github.com/en/codespaces/setting-up-your-project-for-codespaces/setting-up-your-repository/facilitating-quick-creation-and-resumption-of-codespaces)
  - [ ] a link to the Codespaces help documentation
  - [ ] a URL to the Codespaces homepage

#### d306. Tamara is a developer that uses both Visual Studio Codes and Codespaces to manage her code. Tamara has special needs from her environment and has customized her Visual Studio Code settings, and she likes to duplicate those settings across all her development enviroments/machines. How can Tamara synchronize settings across GitHub Codespaces and VS Code?
  - [ ] Tamara should export her settings to a file
  - [ ] Tamara should use a Dotfiles repository (e.g., .bash_profile and .bashrc)
  - [x] Tamara should use Settings Sync feature in Visual Studio Code. Settings Sync enables her to synchronize VS Code settings between the desktop application and the VS Code web client, ensuring a consistent development environment across all her Codespaces

**Exam Notes:**
|You can stop a codespace at any time. When you stop a codespace, any running processes are stopped. Any saved changes in your codespace will still be available when you next start it. The terminal history is preserved, but the visible contents of the terminal window are not preserved between codespace sessions.|
|---|


## Advanced Git Operations and GitHub Features
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

#### 121. You want to merge changes from branch feature-a into main and you are creating a pull request. Which branch should be the base branch and which branch should be the compare branch?
  - [x] main is the base branch and feature-a is the compare branch
  - [ ] feature-a is the base branch and main is the compare branch

#### 122. [How can you link a pull request to an issue? (Select 3.)](https://docs.github.com/en/issues/tracking-your-work-with-issues/linking-a-pull-request-to-an-issue)
  - [x] Linking a pull request to an issue using a keyword (e.g., close #12, closes #12, fix #12, fixes #12, resolve#12)
  - [x] Manually linking a pull request to an issue using the pull request sidebar
  - [x] Manually linking a pull request or branch to an issue using the issue sidebar
  - [ ] By including the issue number in the commit message (incorrect - the keyword should be in the PR description, not the commit message)

**Exam Note:**
|You can link a pull request or branch to an issue to show that a fix is in progress and to automatically close the issue when the pull request or branch is merged.|
|---|

#### 123. What is the effect of adding a line "Closes #11" to the pull request's description?
  - [ ] That PR will be automatically merged on the 11th of that month
  - [ ] Once that PR is merged, the #11th branch will be deleted automatically
  - [ ] That PR will automaticallyl merge once issue #11 is closed
  - [x] Once the PR is merged, issue #11 will be closed automatically

#### 124. What are the possible statuses for a "pull request review"? (Choose three.)
  - [x] Comment: Submit general feedback without explicitly approving the changes or requesting additional changes.
  - [ ] Applaud
  - [x] Approve: Submit feedback and approve merging the changes proposed in the pull request
  - [ ] Deny
  - [x] Request Changes: Submit feedback that must be addressed before the pull request can be merged
  - [ ] Close

[About pull request reviews](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/about-pull-request-reviews)

#### 125. What is the GitHub Sponsor program?
  - [ ] It's a group of companies that fund GitHub
  - [ ] It's a program where highly skilled developers volunteer to help students learn how to use GitHub
  - [ ] It's a program that helps people find a job in the tech industry
  - [x] it's a way to financially suppor the developers of the open source projects.

#### 126. On your personal GitHub dashboard you received a notification that user octocat has created a new repository octocat/my-repo. Why did you receive that notification?
  - [ ] Because you starred the octocat/my-repo repository
  - [ ] Because you recently visited octocat user profile
  - [x] Because you are following the user octocat
  - [ ] Because you contributed to the octocat/my-repo repository

#### 127. What are the GitHub's slash commands?
  - [ ] it's a way of automating GitHub Actions.
  - [ ] It's a way to quickly fix code formatting issues in your PR's code changes
  - [x] [It's a way to quickly insert complex markdown into your PR or issue comments and descriptions.](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-slash-commands)
  - [ ] It's another name for GitHub CLI

**Exam Notes:**

|You can use slash commands in any description or comment field in issues, pull requests, or discussions where that slash command is supported.|
|---|
