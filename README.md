Minimal Java web application displaying the Bright Mind Tech welcome page.

## Features
- Simple gray background with blue welcome message
- Copyright footer
- Maven-based build system
- Ready for Jenkins CI/CD deployment

## Quick Start
```bash
mvn clean package   # Builds brightmind-tech.war
Deployment
Copy target/brightmind-tech.war to Tomcat's webapps/ directory

Access at: http://localhost:8080/brightmind-tech/

Project Structure
brightmind-tech/
├── src/
│   └── main/
│       └── webapp/
│           ├── WEB-INF/
│           │   └── web.xml
│           └── index.html
└── pom.xml
CI/CD Ready
Configure Jenkins to:

Pull from this repository

Build with mvn clean package

Deploy to Tomcat using the "Deploy to container" plugin