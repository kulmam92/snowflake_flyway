Snowflake CI/CD using Flyway and Azure DevOps Pipeline
======================================================

In this post, I’ll discuss how to implement CI/CD pipeline for Snowflake
using Flyway and Azure DevOps Pipeline. This is an advanced topic that
requires a good understanding of various components and concepts.
However, I will try to make it as simple as possible so that people with
minimal DevOps experience can follow this guide and create a working
example. I created the two Github repositories below for that purpose.

-   [kulmam92/snowflake_flyway](https://github.com/kulmam92/snowflake_flyway) - Common
    modules to help set up the Snowflake CI/CD using flyway and Azure
    DevOps pipeline.

-   [kulmam92/flyway-azure](https://github.com/kulmam92/flyway-azure) - flyway
    docker image for the azure pipeline. The official flyway docker
    image can't be used with the Azure DevOps pipeline due to its
    container requirement.

This post consists of three major parts.

-   [Before You Start](01.before_you_start.md)

    -   Basic concepts
        -   This will equip you with the basic concepts about the database deployment and components used in the demo implementation.

    -   Implementation Plan
        -   Explain the design choices

-   [Step-by-Step Implementation](02.step_by_step_implementation.md)
    -   A step-by-step guide that lets you create a working Azure DevOps
        Pipeline using common modules
        from [kulmam92/snowflake_flyway](https://github.com/kulmam92/snowflake_flyway).

-   [Implementation Details](03.iplementation_details.md)
    -   The common modules
        of [kulmam92/snowflake_flyway](https://github.com/kulmam92/snowflake_flyway) will
        be explained.

References
==========

I'm putting references for all subdocuments here.

-   Templates
    -   [kulmam92/snowflake_flyway](https://github.com/kulmam92/snowflake_flyway)
    -   [kulmam92/flyway-azure](https://github.com/kulmam92/flyway-azure)
-   Azure Pipelines
    -   [Azure Pipelines
        documentation](https://docs.microsoft.com/en-us/azure/devops/pipelines/?view=azure-devops)
    -   [CI, CD, YAML &
        Classic](https://docs.microsoft.com/en-us/azure/devops/pipelines/get-started/pipelines-get-started?view=azure-devops)
    -   [Configuring CI/CD Pipelines as Code with YAML in Azure
        DevOps](https://www.azuredevopslabs.com/labs/azuredevops/yaml/)
    -   [Release
        pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/release/?view=azure-devops)
    -   [Releases in Azure
        Pipelines](https://docs.microsoft.com/en-us/azure/devops/pipelines/release/releases?view=azure-devops)        
    -   Variable
        -   [Logging command: set
            variable](https://docs.microsoft.com/en-us/azure/devops/pipelines/scripts/logging-commands?view=azure-devops&tabs=bash#setvariable-initialize-or-modify-the-value-of-a-variable)
        -   [Set secret
            variables](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/variables?view=azure-devops&tabs=yaml%2Cbatch#secret-variables)
        -   [Understanding Azure DevOps Variables \[Complete
            Guide\]](https://adamtheautomator.com/azure-devops-variables-complete-guide/)
        -   [Learn to Use Variable Groups in Azure DevOps
            Pipelines](https://medium.com/slalom-technology/learn-to-use-variable-groups-in-azure-devops-pipelines-203a485b4731)
        -   [Updating Variable Groups From An Azure DevOps
            Pipeline](https://cloudarchitected.com/2019/10/updating-variable-groups-from-an-azure-devops-pipeline/)
    -   Approval
        -   [Azure DevOps Multi-Stage Pipelines Approval
            Strategies](https://devkimchi.com/2019/10/02/azure-devops-multi-stage-pipelines-approval-strategies/)
    -   Template
        -   [Template types & usage](https://docs.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops)
        -   [Solving the looping problem in Azure DevOps
            Pipelines](https://mattvsts.github.io/2019/05/04/solving-the-looping-problem-in-Azure-DevOps-Pipelines/)
        -   [Use Task Groups for better continuous integration
            pipelines](https://medium.com/@izzmo/use-task-groups-for-better-continuous-integration-pipelines-8de4831b0f0f)
-   Flyway
    -   [Flyway
        Migrations](https://flywaydb.org/documentation/migrations#versioned-migrations)

 | [Next >>](01.before_you_start.md)