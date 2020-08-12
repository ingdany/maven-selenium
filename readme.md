# Maven-Selenium
This is a Maven Project using Selenium
## Install Java
1. Install default-jdk
```
sudo apt-get update
sudo apt-get install default-jdk
```
2. Add it to your path 
`export PATH=/usr/lib/jvm/java-11-openjdk-amd64/bin:$PATH`
3. Check if works
`java -version`
## Install Maven
1. Download Maven, because i'm using Ubuntu i will download binary .tar.gz
https://maven.apache.org/download.cgi
2. Extract it
`tar xvfz apache-maven-3.6.3-bin.tar.gz`
3. Add your folder to your PATH
`export PATH=~/apache-maven-3.6.3/bin:$PATH`
4. Confirm if already exist in PATH
`echo $PATH`
5. Now check if work following bash
`mvn -v`
## Create Maven Project
1. In my case i like to work with VS Code, so you should download Java Extension Pack and Maven for Java.
2. Create Maven Project: archetype-quickstart-jdk8 (will ask groupid, artifactid, version, package )
3. Right click below in the Maven section, pick Test
4. Will ask you to add your executable path, go to settings and type following.
`~/apache-maven-3.6.3/bin/mvn`
## Add Selenium to Maven Project
1. Go to https://www.selenium.dev/maven/ , get your dependency and copy to your *pom.xml*
```
<dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version>3.141.59</version>
    </dependency>
```
## Add JUnit to Maven Project
1. Go to https://junit.org/junit4/dependency-info.html and get your dependency, add it to your *pom.xml*
```
<dependency>
  <groupId>junit</groupId>
  <artifactId>junit</artifactId>
  <version>4.13</version>
</dependency>
```