# IBM Business Automation Manager Open Editions (BAMOE) Skills Academy - My Labs

# Overview
This repository includes all labs created by the student during the `BAMOE Skills Academy`.

# Setting up for your labs
In order to have a place to put the labs that you work on during the training, you will need to create your own branch of the repository.  Be sure to select a unique name, such as your name (no spaces).  In a terminal window:

```shell
cd /home/ibmuser/bamoe-skills-academy/bamoe-skills-academy-mylabs
git checkout -b your-unique-branch-name
git push
```

Now, this repository will be the place that you create all your labs for the training.  This is your branch, please do not push to **main**, only to your branch.  

# Guidelines
Use the supplied [Maven Archetypes](../bamoe-maven/README.md) in order to generate the lab project of your choice.  You can emplly a `multi-module` approach to your labs, creating a project for each appliation and then creating a master `pom.xml` that builds all of them in one step.  For example:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
	<modelVersion>4.0.0</modelVersion>

	<groupId>com.ibm.edu.bamoe.labs</groupId>
	<artifactId>bamoe-mylabs</artifactId>
	<version>1.0.0</version>
	<packaging>pom</packaging>

	<!-- Add a <module> for each lab project you create here -->
	<modules>
        <module>my-process-service</module>
        <module>my-decision-service</module>
	</modules>
</project>
```


