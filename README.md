# 🌐 Custom .NET C# Web Server

A lightweight, high-performance **web server built completely from scratch using .NET C#** — with no external frameworks or libraries.  
This project demonstrates the inner workings of HTTP communication, socket-level networking, and multithreaded request handling.  
It’s built to help understand the real mechanics behind how web servers process and respond to client requests.

---

## 🎥 Project Demo
https://github.com/user-attachments/assets/dc02a6ea-47c3-4895-a9ff-15c8f015cedd




---

## 🖼️ Project Screenshots

## [Request Console]  
![Request Console]<img width="1208" height="88" alt="console" src="https://github.com/user-attachments/assets/3d631ce9-fc1c-46e6-b029-003c6ee81128" />


## [Browser Response]  
![Browser Response]<img width="1876" height="402" alt="browser-res" src="https://github.com/user-attachments/assets/20c4ee17-da04-4e74-a710-66eca77df719" />



---

## ✨ Features

- ⚡ Fully functional HTTP 1.1 request and response handling  
- 🧵 Multithreaded client connection management  
- 📁 Serves static files (HTML, CSS, JS, images)  
- 🧠 Simple routing system for GET and POST methods  
- 📜 Custom server logging for each incoming request  
- 🚦 Graceful shutdown and exception handling  
- 💡 Built entirely using `System.Net.Sockets` for raw TCP communication  

---

## Components and working

- Custom request routing for GET, POST, PUT, and DELETE
- Static file serving for HTML, CSS, JavaScript, and image formats
- Default page loading with automatic /index.html fallback
- Pluggable route handlers with Anonymous, Authenticated, and AuthenticatedExpirable behaviors
- Session manager keyed by client IP with authentication state and expiration
- CSRF token generation and validation with hidden form injection
- Error page handling via OnError callback redirects
- Response abstraction supporting redirects, content type, status code, and raw body data
- Multithreaded connection handling with semaphore-based concurrency limits
- Custom HTML post-processing pipeline for runtime injection of tokens and dynamic content

---

## ⚙️ Installation

### Prerequisites

Make sure you have:
- [.NET 8 SDK or newer](https://dotnet.microsoft.com/en-us/download)
- Visual Studio 2022 (or VS Code with the C# Dev Kit)
- Git

### Steps

Open with administrator priviliges to allow the ports


```bash

# Clone this repository
git clone https://github.com/mangothecat07/webserver.git

# Navigate into the project folder
cd webserver

# Restore dependencies
dotnet restore

# Build the project
dotnet build

# Run the server
dotnet run
