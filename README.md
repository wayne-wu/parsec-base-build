# Parsec Base Build
The base build provides a parent [parsec.gradle](https://github.com/wayne-wu/parsec-base-build/blob/master/src/main/resources/parsec.gradle)
file for any Parsec project to inherit from. The build file includes
dependencies, build plugins, and necessary configurations that are used within a Parsec project. These external settings
are designed to enforce a standardized build process in which enhances the quality of the Parsec client's application.
It also includes the Parsec Gradle Plugin which is responsible for parsing the RDLs and generating files.

## Usage
The base build is essentially a Script Plugin and must be inherited using:
```
apply from: 'https://dl.bintray.com/wayne-wu/Gradle/parsec-base-build/1.0.1/parsec.gradle'
```

The parsec.gradle file includes all necessary dependencies for you to get started with a Parsec project.

## Properties
To override properties (eg. version numbers), create identically-named properties within your project. There are multiple
ways of doing this, the easiest way is to add in the properties in your project's `gradle.properties` file. Once you have
define the properties, it will take precedence over the properties defined by the base build.

You can view the defined properties [here](https://github.com/wayne-wu/parsec-base-build/blob/master/src/main/resources/gradle.properties)

