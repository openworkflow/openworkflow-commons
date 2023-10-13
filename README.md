# openworkflow commons

[![Maven Central](https://maven-badges.herokuapp.com/maven-central/co.openworkflow.commons/openworkflow-commons-bom/badge.svg)](https://maven-badges.herokuapp.com/maven-central/co.openworkflow.commons/openworkflow-commons-bom)


openworkflow commons is a collection of shared libraries used by openworkflow open source projects.

## List of libraries

* [openworkflow commons logging][logging]
* [openworkflow commons utils][utils]
* ~~openworkflow commons typed values~~ - migrated to [openworkflow-bpm-platform][typed-values]


## Getting started

If your project is a maven project, start by importing the `openworkflow-commons-bom`.
This will ensure that your project uses all commons libraries in the same version:

```xml
<dependencyManagement>
  <dependencies>
    <dependency>
      <groupId>co.openworkflow.commons</groupId>
      <artifactId>openworkflow-commons-bom</artifactId>
      <version>${version}</version>
      <type>pom</type>
      <scope>import</scope>
    </dependency>
  </dependencies>
</dependencyManagement>
```

Now you can reference individual commons projects:

```xml
<dependency>
  <groupId>co.openworkflow.commons</groupId>
  <artifactId>openworkflow-commons-logging</artifactId>
</dependency>
```

## FAQ

### Which Java (JRE) Version is required?

Java JRE 1.8+ is required.

## License:

The source files in this repository are made available under the <a href="LICENSE">Apache License, Version 2.0</a>.

[logging]: logging/
[utils]: utils/
[typed-values]: https://github.com/openworkflow/openworkflow-bpm-platform/tree/master/typed-values
