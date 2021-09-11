# CI-Junit-Jenkins

Steps to implement contnous integration with Maven project and Junit in Jenkins-

```

1. Create a Jenkins Project-
$ mvn archetype:generate -DgroupId=jenkinsDemo -DartifactId=jenkinsDemo -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

2. Add the below dependency in pom.xml file-

<dependency>
<groupId>junit</groupId>
<artifactId>junit</artifactId>
<version>4.12</version>
</dependency>
<dependency>
<groupId>org.seleniumhq.selenium</groupId>
<artifactId>selenium-java</artifactId>
<version>3.10.0</version>
</dependency>

3. Delete the src/main folder using the commands given below:
$ cd /home/labsuser/jenkinsDemo/src
$ rm -r main

4. Considering you are in the src folder, navigate to src/test/java, and create a file JenkinsDemo.java using the following commands with the code in Git repo:
$ cd /home/labsuser/jenkinsDemo/src/test/java
$ vi JenkinsDemo.java

5. Run the following command to delete any unnecessary files or folder structures:
$ rm -r jenkinsDemo

6. Create a Maven job and add the Build section of your job, for Root POM give the path of the pom.xml in your local system as shown: 
</home/labsuser/jenkinsDemo/pom.xml>

7. Build the job and view the console output.

```






