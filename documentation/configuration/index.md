---
layout: documentation
menu: configuration
menu: configuration
pill: configuration
subtitle: configuration
---

# Configuration

Flyway has many different parameters that can be set to configure its behavior. These parameters can be set through a variety of different means, depending on how you are using Flyway.

## Usage

### Command Line
If using the command line, config parameters can be set via command line arguments (e.g. `./flyway -url=jdbc:h2:mem:flyway info`), [configuration files](/documentation/configfiles), or environment variables (e.g. `FLYWAY_URL=jdbc:h2:mem:flyway`).

### Api
If using the api, config parameters can be set via calling methods on the configuration object returned by `Flyway.configure()` (e.g. `Flyway.configure().url("jdbc:h2:mem:flyway").load()`), [configuration files](/documentation/configfiles), or environment variables if the `.envVars()` method is called on the configuration object.

### Maven
If using maven, config parameters can be set on the configuration xml block in the maven config, [configuration files](/documentation/configfiles), or environment variables (e.g. `FLYWAY_URL=jdbc:h2:mem:flyway`).

### Gradle
If using maven, config parameters can be set in the plugin configuration block, [configuration files](/documentation/configfiles), or environment variables (e.g. `FLYWAY_URL=jdbc:h2:mem:flyway`).

## Parameters

### Connection
- [url](/documentation/configuration/url)
- [user](/documentation/configuration/user)
- [password](/documentation/configuration/password)
- [driver](/documentation/configuration/driver)
- [connectRetries](/documentation/configuration/connectRetries)
- [initSql](/documentation/configuration/initSql)
- [jdbcProperties](/documentation/configuration/jdbcProperties) {% include teams.html %}

### General

- [batch](/documentation/configuration/batch) {% include teams.html %}
- [callbacks](/documentation/configuration/callbacks)
- [cherryPick](/documentation/configuration/cherryPick) {% include teams.html %}
- [configFileEncoding](/documentation/configuration/configFileEncoding)
- [configFiles](/documentation/configuration/configFiles)
- [dryRunOutput](/documentation/configuration/dryRunOutput) {% include teams.html %}
- [encoding](/documentation/configuration/encoding)
- [errorOverrides](/documentation/configuration/errorOverrides) {% include teams.html %}
- [group](/documentation/configuration/group)
- [installedBy](/documentation/configuration/installedBy)
- [jarDirs](/documentation/configuration/jarDirs)
- [licenseKey](/documentation/configuration/licenseKey) {% include teams.html %}
- [locations](/documentation/configuration/locations)
- [mixed](/documentation/configuration/mixed)
- [outOfOrder](/documentation/configuration/outOfOrder)
- [outputQueryResults](/documentation/configuration/outputQueryResults) {% include teams.html %}
- [skipDefaultCallbacks](/documentation/configuration/skipDefaultCallbacks)
- [skipDefaultResolvers](/documentation/configuration/skipDefaultResolvers)
- [skipExecutingMigrations](/documentation/configuration/skipExecutingMigrations) {% include teams.html %}
- [stream](/documentation/configuration/stream) {% include teams.html %}
- [table](/documentation/configuration/table)
- [tablespace](/documentation/configuration/tablespace)
- [target](/documentation/configuration/target)
- [validateMigrationNaming](/documentation/configuration/validateMigrationNaming)
- [validateOnMigrate](/documentation/configuration/validateOnMigrate)
- [workingDirectory](/documentation/configuration/workingDirectory)

### Schema
- [createSchemas](/documentation/configuration/createSchemas)
- [defaultSchema](/documentation/configuration/defaultSchema)
- [schemas](/documentation/configuration/schemas)

### Baseline
- [baselineDescription](/documentation/configuration/baselineDescription)
- [baselineOnMigrate](/documentation/configuration/baselineOnMigrate)
- [baselineVersion](/documentation/configuration/baselineVersion)

### Clean
- [cleanDisabled](/documentation/configuration/cleanDisabled)
- [cleanOnValidationError](/documentation/configuration/cleanOnValidationError)

### Validate
- [ignoreFutureMigrations](/documentation/configuration/ignoreFutureMigrations)
- [ignoreIgnoredMigrations](/documentation/configuration/ignoreIgnoredMigrations)
- [ignoreMissingMigrations](/documentation/configuration/ignoreMissingMigrations)
- [ignorePendingMigrations](/documentation/configuration/ignorePendingMigrations)

### Migrations
- [repeatableSqlMigrationPrefix](/documentation/configuration/repeatableSqlMigrationPrefix)
- [resolvers](/documentation/configuration/resolvers)
- [sqlMigrationPrefix](/documentation/configuration/sqlMigrationPrefix)
- [sqlMigrationSeparator](/documentation/configuration/sqlMigrationSeparator)
- [sqlMigrationSuffixes](/documentation/configuration/sqlMigrationSuffixes)
- [undoSqlMigrationPrefix](/documentation/configuration/undoSqlMigrationPrefix) {% include teams.html %}

### Placeholders
- [placeholderPrefix](/documentation/configuration/placeholderPrefix)
- [placeholderReplacement](/documentation/configuration/placeholderReplacement)
- [placeholders](/documentation/configuration/placeholders)
- [placeholderSuffix](/documentation/configuration/placeholderSuffix)

### Command Line
- [color](/documentation/configuration/cliColor)
- [edition](/documentation/configuration/edition)

### Oracle
- [oracleSqlPlus](/documentation/configuration/oracleSqlPlus) {% include teams.html %}
- [oracleSqlPlusWarn](/documentation/configuration/oracleSqlPlusWarn) {% include teams.html %}