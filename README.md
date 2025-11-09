# 🧪 Selenium Automation Framework (Java + Maven + TestNG)

> A modular automation framework built using **Java**, **Selenium WebDriver**, **Maven**, and **TestNG**, following the **Page Object Model (POM)** design pattern.

This framework automates web UI testing for login and homepage functionality.  
It includes reusable Page Object classes, test scripts, and a structured Maven project setup.

---

## ⚙️ Tech Stack
- **Language:** Java  
- **Testing Framework:** TestNG  
- **Build Tool:** Maven  
- **Automation Library:** Selenium WebDriver  
- **Design Pattern:** Page Object Model (POM)  
- **IDE:** Eclipse / IntelliJ IDEA  

---

## 📦 Maven Dependencies

All dependencies are managed through `pom.xml`.  
Typical dependencies used in this project include:

```xml
<dependencies>
    <!-- Selenium WebDriver -->
    <dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version><!-- your selenium version --></version>
    </dependency>

    <!-- TestNG -->
    <dependency>
        <groupId>org.testng</groupId>
        <artifactId>testng</artifactId>
        <version><!-- your testng version --></version>
        <scope>test</scope>
    </dependency>

    <!-- (Optional) WebDriverManager for driver binaries -->
    <!--
    <dependency>
        <groupId>io.github.bonigarcia</groupId>
        <artifactId>webdrivermanager</artifactId>
        <version><!-- your wdm version --></version>
    </dependency>
    -->
</dependencies>
You can update the versions as needed directly in pom.xml.

📂 Project Structure
text
Copy code
Selenium-Automation-Framework/
│
├── pom.xml                 # Maven dependencies and build configuration
│
├── src/
│   ├── main/java/
│   │   ├── HomePage.java       # POM class for homepage elements & actions
│   │   ├── SignInPage.java     # POM class for login/sign-in actions
│   │   ├── LoginPOM.java       # Common POM or login utility class
│   │   └── Demo.java           # Driver / utility / base setup
│   │
│   └── test/java/
│       └── Tests.java          # TestNG test cases for UI validation
│
└── .gitignore
```
🚀 How to Run Tests
Clone the repository
```
bash
git clone https://github.com/Mus-1/Selenium-Automation-Framework.git
cd Selenium-Automation-Framework
```

Run tests using Maven
```
bash
mvn clean test
```
View reports
TestNG reports will be generated under:
```
target/surefire-reports/
```

💡 Features

✅ Page Object Model (POM) implementation

✅ Modular and maintainable code structure

✅ Maven-based dependency and build management

✅ Easy to extend for new test cases and pages

✅ Ready for CI tools like Jenkins / GitHub Actions
