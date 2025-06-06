# Task 8: Run a Simple Java Maven Build Job in Jenkins

## ✅ Objective
To use Jenkins to build a basic Java application using Maven as part of a CI/CD pipeline.

## 🛠 Tools Used
- Jenkins (running as a system service on AWS EC2)
- Java 17
- Apache Maven 3.6.3
- Ubuntu (EC2 instance)

## 📁 Project Structure
task-8-java-maven/
├── pom.xml
└── src/
└── main/
└── java/
└── HelloWorld.java

## 📄 File Descriptions

### `HelloWorld.java`
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, Jenkins + Maven!");
    }
}
pom.xml
Maven Project Object Model file used to compile the Java app:

Sets Java source/target to 1.8

Uses maven-compiler-plugin version 3.8.1

⚙️ Jenkins Job Configuration
Project Type: Freestyle

Build Step: Invoke top-level Maven targets

Goals: clean package

Maven Version: Maven-3.6.3 (configured in Global Tool Configuration)

Source Code Management: Local workspace (copied manually)

🚀 Steps Performed
Installed Java 17 and Maven 3.6.3 on EC2 instance

Created a simple Java HelloWorld project with pom.xml

Set up Jenkins Freestyle project

Configured Maven build step with goal clean package

Built the job and got BUILD SUCCESS in the console output

📸 Screenshot
Included in this repo: screenshot.png showing BUILD SUCCESS in Jenkins console output.


