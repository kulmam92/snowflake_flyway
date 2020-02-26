# Introduction
This repository contains two things.

* Sample flyway migration script for database "flyway_demo".
* Common modules that can be used to set up Azure DevOps pipeline for Snowflake deployment using flyway.


Refer to the below page for Step-by-Step instructions on how to use this.

[Snowflake CI/CD using Flyway and Azure DevOps Pipeline](/docs/index.md)

# Getting Started
The below are incldued files.
```
├── README.md
├── LICENSE
├── databases
│   ├── README.md
│   └── flyway_demo
│       ├── V20200120.1__SCHEMA_DEMO_Create.sql
│       ├── V20200120.2__TABLE_DEMO.DEMOTABLE_Create.sql
│       ├── V20200123.1__TABLE_DEMO.DEMOTABLE_Alter.sql
│       └── view
│           └── R__VIEW_DEMO.V_DEMOVIEW.sql
└── templates
    ├── README.md
    ├── TaskGroups
    ├── VariableGroups
    │   ├── Classic
    │   │   └── Snowflake.Database.env      <- Variable group for Classic pipeline
    │   └── YAML
    │       └── Snowflake.Database.env      <- Variable group for YAML pipeline
    └── YAMLpipelines
        ├── azure-pipelines.yml             <- YAML pipeline script
        └── templates
            ├── snowflakeFlywayBuild.yml    <- YAML pipeline template for snowflake build using flyway
            └── snowflakeFlywayDeploy.yml   <- YAML pipeline template for snowflake deploy using flyway
```