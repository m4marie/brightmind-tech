# 🚀 Bright Mind Tech Web Application  

<div align="center">
  
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Maven](https://img.shields.io/badge/Apache%20Maven-C71A36?style=for-the-badge&logo=Apache%20Maven&logoColor=white)
![Tomcat](https://img.shields.io/badge/Apache%20Tomcat-%23F8DC75?style=for-the-badge&logo=apache-tomcat&logoColor=black)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=Jenkins&logoColor=white)

</div>

## 🌟 Features  
- 🎨 **Clean UI**: Gray background with <span style="color:#00BFFF">deep sky blue</span> welcome message  
- ©️ **Professional footer** with BMT 2025 copyright  
- 🛠️ **Maven-powered** build system  
- ⚡ **CI/CD ready** for Jenkins automation  

## 🛠️ Tech Stack  
| Component       | Technology |
|----------------|------------|
| Backend        | Java Servlet API |
| Build Tool     | Apache Maven |
| Web Server    | Apache Tomcat 9+ |
| CI/CD         | Jenkins |

## 🚀 Quick Start  
```bash
# Clone repository
git clone https://github.com/yourusername/brightmind-tech.git

# Build WAR file
cd brightmind-tech
mvn clean package

🚀 Deployment
Copy target/brightmind-tech.war to Tomcat's webapps/ directory

Access at: http://localhost:8080/brightmind-tech/

📂 Project Structure

brightmind-tech/
├── src/
│   └── main/
│       └── webapp/
│           ├── WEB-INF/
│           │   └── web.xml
│           └── index.html
└── pom.xml

🔄 CI/CD Pipeline

    A[GitHub] -->|Pull| B(Jenkins)B -->|Build| C[WAR File]C -->|Deploy| D[Tomcat]

License
© 2025 Bright Mind Tech