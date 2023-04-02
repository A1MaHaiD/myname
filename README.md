### **Maven phases**

1. validate: validate the project is correct and all necessary information is available
2. compile: compile the source code of the project
3. test: test the compiled source code using a suitable unit testing framework. These tests should not require the code be packaged or deployed
4. package: take the compiled code and package it in its distributable format, such as a JAR.
5. verify: run any checks to verify the package is valid and meets quality criteria
6. install: install the package into the local repository, for use as a dependency in other projects locally
7. deploy: done in an integration or release environment, copies the final package to the remote repository for sharing with other developers and projects.

---

**There are two other Maven lifecycles of note beyond the default list above. They are:**

* clean: cleans up artifacts created by prior builds
* site: generates site documentation for this project

---

### **Maven dependency scopes:**

* compile - This is the default scope, used if none is specified.
* provided - This is much like compile, but indicates you expect the JDK or a container to provide the dependency at runtime.
* runtime - This scope indicates that the dependency is not required for compilation, but is for execution.
* test - This scope indicates that the dependency is not required for normal use of the application.
* import - This scope is only supported on a dependency of type pom in the section.
