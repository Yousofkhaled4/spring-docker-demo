# Spring Boot Docker App

This is a simple Java Spring Boot application that runs inside a Docker container.

## 🛠️ Technologies Used

- Java 17
- Spring Boot
- Maven
- Docker

---

## 📦 How to Build the App

Make sure you have Maven installed, then run:


```bash

mvn clean package -DskipTests

```

This will generate a `.jar` file inside the `target/` directory.

---

## 🐳 How to Build Docker Image

Use the following command to build the Docker image:

```bash

docker build -t spring-demo .

```

---

## ▶️ How to Run the Container

Run the container and map port 8080:


```bash

docker run -d -p 8080:8080 --name spring-container spring-demo

```

You can now access the app at:

```
http://localhost:8080

```

---

## 🛑 How to Stop and Remove the Container

```bash
docker stop spring-container
docker rm spring-container
```

---

## 📁 Project Structure

```
.
├── Dockerfile
├── README.md
├── pom.xml
└── src/
```

---

## ✍️ Author

Yousof Khaled

