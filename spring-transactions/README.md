spring-transactions: demonstrates how to combine multiple Enterprise Integration Patterns to solve integration problems
===================================
Author: Fuse Team  
Level: Beginner  
Technologies: Spring,Blueprint  
Summary: Demonstrates how to get a reference to the container provided Spring Transaction Manager
Target Product: Fuse  
Source: <https://github.com/jboss-fuse/quickstarts>


System requirements
-------------------

Before building and running this example you need:

* Maven 3.0.4 or higher
* JDK 1.6 or 1.7
* JBoss Fuse 6


Build and Deploy the Quickstart
-------------------------------

1. Change your working directory to `spring-transactions` directory.
*. Run `mvn clean install` to build the quickstart.
*. Start JBoss Fuse 6 by running bin/fuse (on Linux) or bin\fuse.bat (on Windows).
*. In the JBoss Fuse console, enter the following command:

        osgi:install -s mvn:org.jboss.quickstarts.fuse/spring-transactions/${project.version}

*. Fuse should give you an id when the bundle is deployed
*. You can check that everything is ok by issuing  the command:

        osgi:list
   your bundle should be present at the end of the list


        ...

Undeploy the Bundle
-------------------

To stop and undeploy the bundle in Fuse:

1. Enter `osgi:list` command to retrieve your bundle id
2. To stop and uninstall the bundle enter

        osgi:uninstall <id>
 

