## Define and implement continuous integration (20-25%)
### Design build automation
- integrate the build pipeline with external tools
    - (e.g., Dependency and security scanning, Code coverage)
- implement quality gates (e.g., code coverage, internationalization, peer review)
- design a testing strategy (e.g., integration, load, fuzz, API, chaos)
- integrate multiple tools (e.g., GitHub Actions, Azure Pipeline, Jenkins)
### Design a package management strategy
- recommend package management tools
    - (e.g., GitHub Packages, Azure Artifacts, Azure Automation Runbooks Gallery, Nuget, Jfrog, Artifactory)
- design an Azure Artifacts implementation including linked feeds
- design versioning strategy for code assets (e.g., SemVer, date based)
- plan for assessing and updating and reporting package dependencies
    - (e.g.: GitHub Automated Security Updates, NuKeeper, GreenKeeper)
- design a versioning strategy for packages (e.g., SemVer, date based)
- design a versioning strategy for deployment artifacts
### Design an application infrastructure management strategy
- assess a configuration management mechanism for application infrastructure
- define and enforce desired state configuration for environments
### Implement a build strategy
- design and implement build agent infrastructure (include cost, tool selection, licenses,
maintainability)
- develop and implement build trigger rules
- develop build pipelines
- design build orchestration (products that are composed of multiple builds)
- integrate configuration into build process
- develop complex build scenarios (e.g., containerized agents, hybrid, GPU)
### Maintain build strategy
- monitor pipeline health (failure rate, duration, flaky tests)
- optimize build (cost, time, performance, reliability)
- analyze CI load to determine build agent configuration and capacity
### Design a process for standardizing builds across organization
- manage self-hosted build agents (VM templates, containerization, etc.)
- create reuseable build subsystems (YAML templates, Task Groups, Variable Groups, etc.)
