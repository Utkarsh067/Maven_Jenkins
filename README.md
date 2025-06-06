# ☕ Hello Java Maven with Jenkins CI

This project demonstrates a simple **Java Maven build** integrated with **Jenkins** using a **Freestyle project**. It prints "Hello, Jenkins + Maven!" and builds with `mvn clean package`.

---

## 📂 Project Structure
```
hello-java-maven/
├── pom.xml
└── README.md
└── HelloWorld.java
```

---

## ⚙️ Jenkins CI Configuration
Jenkins Setup:
+ Jenkins installed via Docker:
  ```
  docker run -p 8080:8080 -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts
  ```

+ Installed tools via Manage Jenkins → Tools Configuration:

    - Maven 3.8.6

    - Java JDK 8/11

    - Git
 
---

## 🛠️ Jenkins Freestyle Job Setup
1. New Item → hello-java-maven-job → Freestyle project

2. Source Code Management: Git

+ Use repo URL (e.g., https://github.com/your-username/hello-java-maven.git)

3. Build Step:

+ Select: Invoke top-level Maven targets

+ Goals: clean package

+ Maven version: Maven 3.8.6

---

## ✅ Build Output
Successful build output contains:

```BUILD SUCCESS```

📸 Screenshot:


---

✍🏽 Author

Utkarsh Jain

[LinkedIn](https://www.linkedin.com/in/utkarsh-jain02/)
