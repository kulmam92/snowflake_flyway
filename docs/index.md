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