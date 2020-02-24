# Introduction 
Sample flyway migration script for database "flyway_demo".

# Getting Started
The below are incldued scripts.
```
├── README.md
└── flyway_demo
    ├── V20200120.1__SCHEMA_DEMO_Create.sql
    ├── V20200120.2__TABLE_DEMO.DEMOTABLE_Create.sql
    ├── V20200123.1__TABLE_DEMO.DEMOTABLE_Alter.sql
    └── view
        └── R__VIEW_DEMO.V_DEMOVIEW.sql
```

## Migration script type
### Versioned
Versioned migration script is when you need to apply change scripts in order exactly once.
Each versioned migration has a version, a description and a checksum. The description is purely informative for you to be able to remember what each migration does. The checksum is there to detect accidental changes.

### Naming Convention
This is an example naming convention that I came up for the demo database. You may create your own naming convention based on your need.
```
V[RealseDate].[Sequence]__[ObjectType]_[Schema].[ObjectName]_[Create|Drop|Alter].sql
```

#### Folder structure
```
databases\[DatabaseName]\MingrationScript.sql
```

### Repeatable
Repeatable migration script is used to manage database objects like view whose definition can then simply be maintained in a single file in version control. Flyway uses a checksum to detact changes.

### Naming Convention
```
R__[ObjectType]_[Schema].[ObjectName].sql
```

#### Folder structure
```
databases\[DatabaseName]\[ObjectType]\MingrationScript.sql
```
