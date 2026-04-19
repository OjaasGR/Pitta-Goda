# 💬 Real-Time Chat Application

A simple real-time chat application built using **Spring Boot** and **WebSocket (STOMP)** that enables bidirectional communication between clients and the server.

---

## 🚀 Features

* Real-time messaging using WebSockets
* STOMP protocol for message handling
* Join/leave notifications
* Multiple users can chat simultaneously
* Lightweight frontend using HTML, CSS, and JavaScript
* Session-based user tracking

---

## 🛠️ Tech Stack

* **Backend:** Spring Boot
* **WebSocket:** STOMP Protocol
* **Frontend:** HTML, CSS, JavaScript
* **Build Tool:** Maven

---

## ⚙️ How It Works

* WebSocket endpoint is exposed at:

  ```
  /ws
  ```
* Messages are sent to:

  ```
  /app/chat.sendMessage
  ```
* Users join via:

  ```
  /app/chat.addUser
  ```
* Messages are broadcasted to:

  ```
  /topic/public
  ```

---

## 📂 Project Structure

```
src/
 ├── main/
 │   ├── java/com/Ojas/chat/
 │   │   ├── config/
 │   │   │   ├── WebSocketConfig.java
 │   │   │   └── WebSocketEventListener.java
 │   │   ├── chat/
 │   │   │   ├── ChatController.java
 │   │   │   ├── ChatMessage.java
 │   │   │   └── MessageType.java
 │   │   └── ChatApplication.java
 │   └── resources/
 │       └── static/
 │           ├── index.html
 │           ├── css/
 │           └── js/
```

---

## ▶️ Running the Application

### 1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

### 2. Run the application

```bash
./mvnw spring-boot:run
```

or (Windows):

```bash
mvnw.cmd spring-boot:run
```

### 3. Open in browser

```
http://localhost:8080
```

---

## 🧠 Key Concepts Used

* WebSocket full-duplex communication
* Message broker (`/topic`)
* Application destination prefix (`/app`)
* STOMP messaging protocol
* Event-driven architecture

---

## 📸 Demo

(Add screenshots here if you want)

---

## 📌 Future Improvements

* Private messaging
* Message persistence (database)
* Authentication & user login
* Typing indicators
* UI improvements

---

## 👨‍💻 Author

Gowtham Roy

---
