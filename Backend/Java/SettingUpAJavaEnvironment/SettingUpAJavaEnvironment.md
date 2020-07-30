# Setting Up a Java Environment - Pluralsight course by Sander Mak
### Module 1 - Course Overview

_Nothing much to note_

---

### Module 2 - Installing and Running Java
Goal
* Install JDK
* Install IDE - IntelliJ
* Have a working environment to build Java apps


To run a simple Java code - you need do 2 things. 
1. Using “javac” compiler convert the .java file to a .class file = byte code. This byte code is system independent - Write Once Run Anywhere (WORA)
2. With the help of Java Standard Edition (SE) APIs (for e.g. “System” class is not defined in our program) + Java Virtual Machine (JVM), execute the byte code. 



JVM + Java SE APIs + tools like java and “javac” is called the JDK Java Development Kit

Another set of APIs called Java Enterprise Edition (EE) APIs - libraries geared towards developing web applications, enterprise application integrations, database access, etc. whereas Java SE APIs are more fundamental such as networking, file access, creating and managing collections in your code and other basic APIs that you expect your application runtime to offer. 

Java EE APIs are not part of the JDK. If you want to build Enterprise Java applications making us of these EE APIs, you’ll need additional tools like an application server that’s on top of the JDK or Java EE APIs for your app. 



Oracle has stopped developing Java EE and has donated all of these APIs to the Eclipse Foundation where it lives on as Jakarta EE. 


Installing the JDK 
_follow along the course_

1. Download latest JDK - https://jdk.java.net
    1. Not compulsory but convention is to place it in Program Files in Windows

_skipping_

---

### Module 3 - Using IntelliJ for Java Development
_skipping_

---

### Module 4 - Packaging Java Applications
* Java apps are packaged into JAR files - "Java ARchive”. It’s just a zip file
* It contains the compiled classes (platform independent byte code generated by a compiler) of your application nicely structured based on their packages
* Also optionally contains meta data - META-INF/MANIFEST.MF
* Creating a JAR file
    * Additional tool present in JDK called “jar"
    * In the output directory containing the classes - “jar cvmf TC-MANIFEST.MF <name>.jar .” “m” specifies which class to treat as main so that JVM will know how to launch.
    * This generates the manifest file as well. 
    * “java -jar <name>.jar” to run the JAR file. 
* While you can manually create jar files, typically it’s done in an automated fashion by build tools (maven, gradle) which you can also use to perform test, static code analysis
    * Build
    * Test
    * Analyse
    * Package

---





