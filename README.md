# 💬 SignalR Chat Application

A real-time chat application built using *ASP.NET Core* and *SignalR*, showcasing live message broadcasting between multiple connected users via a simple web interface.

---

## 📌 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [How It Works](#-how-it-works)

---

## 🚀 Features

- 🔄 Real-time communication using SignalR
- 🌐 Web-based frontend (HTML + JavaScript)
- 🔊 Messages broadcast to all connected users instantly
- 📱 Works across multiple tabs/devices

---

## 🧰 Tech Stack

- *Backend:* ASP.NET Core 9.0, SignalR
- *Frontend:* HTML, CSS, JavaScript
- *IDE (Optional):* Visual Studio 2022 / Visual Studio Code

---

## 📁 Project Structure
SignalRChat/
├── Hubs/
│ └── ChatHub.cs # SignalR hub for real-time messaging
│
├── wwwroot/
│ ├── index.html # Main UI for chat
│ └── chat.js # JS logic for SignalR connection
│
├── Program.cs # Application entry point
└── SignalRChat.csproj # .NET Core project file


---

## ⚙ Getting Started

### Prerequisites

- [.NET 9.0 SDK](https://dotnet.microsoft.com/en-us/download)
- Git (optional)
- Visual Studio or any code editor

*How It Works*

The browser (client) connects to a SignalR Hub on the server.

When a user sends a message:

The message is sent to the ChatHub.cs

The hub broadcasts it to all other connected clients

Clients instantly receive and render the message without page refresh
