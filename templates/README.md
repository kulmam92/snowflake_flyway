# Introduction 
Common modules that can be used to set up Azure DevOps pipeline for Snowflake deployment using flyway.

# Getting Started
```
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