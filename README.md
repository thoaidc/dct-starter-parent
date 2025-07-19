# DCT Spring Boot Starter Parent

---

The `starter-parent` Maven project provides shared configuration and version management for DCT system’s Spring Boot modules.
It helps standardize the build structure, reduce configuration duplication, and ensure consistency across subprojects.
## Key Features

* Centralized version management for:

  * Spring Boot
  * Spring Cloud
  * Popular libraries such as Jackson, Hibernate Validator, ModelMapper, JWT, MySQL driver, etc.
* Preconfigured Maven Plugins: Compiler, Enforcer, Spotless (code formatting), Resources, Surefire, etc.
* Defines minimum required versions of Java and Maven
* Customizable `pluginManagement` for child projects
* Supports flexible overrides in subprojects

## Usage
In the child project's `pom.xml`, inherit it as follows:

```xml
<parent>
  <groupId>com.dct</groupId>
  <artifactId>starter-parent</artifactId>
  <version>${optional-version}</version>
</parent>
