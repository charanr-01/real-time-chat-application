# Real-Time Chat Application

A real-time chat application built with **Java Spring Boot** and **WebSocket**, enabling instant messaging between connected users.

## Features

- Real-time messaging using WebSocket (STOMP over SockJS)
- Multiple users can join and chat simultaneously
- Instant message broadcast to all connected clients
- Lightweight and easy to run locally

## Tech Stack

- **Backend:** Java, Spring Boot
- **Real-time communication:** WebSocket, STOMP
- **Build tool:** Maven

## Prerequisites

- Java 17+ (or your project's JDK version)
- Maven 3.6+

## Getting Started

1. Clone the repository
   ```bash
   git clone https://github.com/charanr-01/real-time-chat-application.git
   cd real-time-chat-application
   ```

2. Build the project
   ```bash
   mvn clean install
   ```

3. Run the application
   ```bash
   mvn spring-boot:run
   ```

4. Open your browser and go to:
   ```
   http://localhost:8080
   ```

## Project Structure

```
├── src/
│   ├── main/
│   │   ├── java/        # Application source code
│   │   └── resources/   # Config files, static assets, templates
├── pom.xml               # Maven build configuration
└── README.md
```

## How It Works

1. Clients connect to the server via a WebSocket endpoint.
2. Messages sent by a client are published to a topic.
3. The server broadcasts the message to all subscribed clients in real time.

## Future Improvements

- User authentication
- Private one-on-one messaging
- Chat history persistence with a database
- Typing indicators and read receipts

## License

This project is open source and available under the [MIT License](LICENSE).
