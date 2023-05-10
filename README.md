# ImGui Sample

This project demonstrates how to build an ImGui example using Nokee plugins for Gradle.
In this sample, both the ImGui library and the application are built together.

## Requirements

To build this project, you will need:

- Java Development Kit (JDK) 8 or above.
- A modern C++ compiler that supports C++17.
- Git installed on your system.

## Getting Started

### Cloning the Repository

To clone the repository including the ImGui submodule, use the following command:

```
git clone --recurse-submodules https://github.com/nokeedev/nokee-samples-imgui
```

### Building the Project

To build the project, navigate into the project root directory (where the `settings.gradle` file is located) and run the following command:

```
./gradlew build
```

This will build both the ImGui library and the example application.
To execute the application, run the following command:

```
./build/exes/main/nokee-samples-imgui
```

## Project Structure

- *src/main/cpp*: This directory contains the source code for the ImGui example application.
- *libs/imgui*: This is a submodule containing the ImGui source code.
- *build.gradle*: This is the Gradle build script, which uses Nokee plugins to build the ImGui library and the example application together.

## Important Details

This sample demonstrates how to build the ImGui library and an application together in a single project.
It's possible to build the ImGui library as a separate Gradle project, using `dev.nokee.cpp-library`, and use it as a dependency in other projects, but this is not demonstrated in this sample.
