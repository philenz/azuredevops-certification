## Manage source control (10-15%)
### Develop a modern source control strategy
- integrate/migrate disparate source control systems (e.g., GitHub, Azure Repos)
- design authentication strategies
- design approach for managing large binary files (e.g., Git LFS)
- design approach for cross repository sharing (e.g., Git sub-modules, packages)
- implement workflow hooks
- design approach for efficient code reviews
    - (e.g., GitHub code review assignments, schedule reminders, Pull Analytics)
### Plan and implement branching strategies for the source code
- define Pull Requests (PR) guidelines to enforce work item correlation
- implement branch merging restrictions (e.g., branch policies, branch protections, manual, etc.)
- define branch strategy (e.g., trunk based, feature branch, release branch, GitHub flow)
- design and implement a PR workflow (code reviews, approvals)
- enforce static code analysis for code-quality consistency on PR
### Configure repositories
- configure permissions in the source control repository
- organize the repository with git-tags
- plan for handling oversized repositories
- plan for content recovery in all repository states
- purge data from source control
### Integrate source control with tools
- integrate GitHub with DevOps pipelines
- integrate GitHub with identity management solutions (Azure AD)
- design for GitOps
- design for ChatOps
- integrate source control artifacts for human consumption (e.g., Git changelog)
- integrate GitHub Codespaces
