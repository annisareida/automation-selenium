# 🧪 Web Automation Testing - Selenium + JUnit

Proyek ini merupakan implementasi **automation testing berbasis web** menggunakan **Selenium WebDriver**, **JUnit 5**, dan **Maven**.  
Pengujian dilakukan pada website open-source: https://www.saucedemo.com/

---

## 🚀 Tech Stack

- Java 21
- Selenium WebDriver
- JUnit 5
- Maven
- WebDriverManager

---

## 📁 Project Structure

```
automation-selenium
├── src
│   ├── main
│   │   └── App.java
│   ├── test
│   └── java
│       ├── base
│       │   └── BaseTest.java
│       ├── pages
│       │   └── LoginPage.java
│       └── test
│           └── LoginTest.java
├── pom.xml
└── README.md
```

---

## 🧩 Features

### ✅ Login Automation Test
- Login dengan kredensial valid
- Validasi redirect ke halaman inventory

### ❌ Negative Test
- Login dengan kredensial salah
- Validasi error message

---

## 🛠️ Setup & Installation

### 1. Clone Repository

```bash
git clone https://github.com/username/automation-selenium.git
cd automation-selenium
```

### 2. Install Dependencies

```bash
mvn clean install
```

### 3. Run Test

```bash
mvn test
```

---

## ▶️ Test Result

Contoh hasil eksekusi:

```
Tests run: 4
Failures: 0
Errors: 0
BUILD SUCCESS
```

---

## 🧪 Sample Test Case

**Valid Login**

```java
loginPage.login("standard_user", "secret_sauce");
assertEquals("https://www.saucedemo.com/inventory.html", driver.getCurrentUrl());
```

**Invalid Login**

```java
loginPage.login("wrong_user", "wrong_pass");
assertEquals("Epic sadface: Username and password do not match any user in this service", error);
```

---

## 📌 Best Practices Used

- Page Object Model (POM)
- Reusable Base Test Class
- Separation of Test Logic & Page Logic
- Automated Driver Management (WebDriverManager)

---

## 👩‍💻 Author

**Annisa Reida Raheima**  
Informatics Engineering Graduate Student  

---
