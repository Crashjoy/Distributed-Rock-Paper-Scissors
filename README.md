# Distributed Rock-Paper-Scissors Game

A networked multiplayer Rock-Paper-Scissors game built in Java, where two
players can play against each other in real time over a network connection.

## What it does

- Real-time peer-to-peer gameplay over TCP/IP sockets
- A multi-threaded server that handles concurrent player connections without
  freezing the UI
- A Swing/AWT interface designed with WCAG accessibility guidelines in mind
- A privacy-policy workflow with persistent user-agreement storage

## Tech stack

- Language: Java
- UI: Java Swing, AWT
- Networking: TCP/IP sockets, Java Networking API
- Concurrency: Java threading (dedicated network listener + UI threads)
- Tools: Eclipse, Git, GitHub

## Why this project exists

I built this to move beyond standard desktop apps and actually learn how
distributed systems work — how two processes connect over a network, how to
manage socket connections for simultaneous players, and how to keep a UI
responsive while network operations run in the background. The hardest part was
getting the threading right so the game stayed responsive during network
communication.

## Project structure

The project is organized into four packages:

- `controller/` — game logic and event handling
- `model/` — game state and data
- `utils/` — TCP/IP networking logic
- `view/` — Swing/AWT graphical interface


## Getting started

Prerequisites: JDK 17+

```bash
git clone <your-repo-url>
cd <repo-folder>
# Compile
javac -d out $(find src -name "*.java")
# Run (server instance)
java -cp out com.aldiyar.rockpaperscissors.view.Main

```
<!--
# 🎮 Distributed Rock-Paper-Scissors

## 📋 Project Overview

A Java-based networked game that enables real-time, peer-to-peer gameplay. This project was engineered to master TCP/IP socket communication, multi-threaded concurrency, and Java Swing/AWT UI design, providing a robust foundation for distributed system development.

## 🚀 The Challenge

The objective was to build a low-latency, multi-threaded gaming environment where two users can compete over a network. The primary challenge was managing socket connections for simultaneous players while ensuring thread safety and a responsive, accessible UI.

## ✨ Key Features
- 🌐 **TCP/IP Socket Networking:** Implemented custom socket communication to facilitate real-time data exchange between two players.
- 🧵 **Multi-threaded Concurrency:** Utilized Java threading to handle concurrent connections, ensuring the UI remains responsive during network operations.
- 🖥️ **Java Swing/AWT UI:** Built a custom graphical interface with focus on WCAG accessibility guidelines for universal usability.
- 🔐 **Privacy & Compliance:** Integrated a robust privacy policy workflow with persistent user-agreement storage.
- 🚀 **Deployment Ready:** Includes a comprehensive Google Play Store submission package, covering data safety, privacy policy documentation, and visual assets.

## 🛠️ Tech Stack
- **Language:** Java
- **UI Framework:** Java Swing, AWT
- **Networking:** TCP/IP Sockets, Java Networking API
- **Concurrency:** Java Threading (Multi-threading)
- **Data Persistence:** Local File I/O (Privacy agreement state)
- **Tools:** Eclipse, Git, GitHub

## 🏗️ System Architecture
- **Client Layer:** Swing/AWT interface handling user input and game state visualization.
- **Networking Layer:** TCP/IP Socket implementation managing peer-to-peer connection and message passing.
- **Threading Layer:** Dedicated threads for network listening and UI rendering, preventing application blocking.
- **Compliance Layer:** Privacy policy manager ensuring user data protection and agreement tracking.

## 📈 Impact & Results
- **Technical Mastery:** Successfully implemented distributed system concepts, moving beyond standard desktop applications into networked environments.
- **Quality Assurance:** Ensured high-level compliance by preparing a full Google Play Store release package, including data safety and privacy documentation.

## 📂 Project Structure
- [/src/com/aldiyar/rockpaperscissors/controller/](https://github.com/Crashjoy/Distributed-Systems-Project/tree/master/src/com/aldiyarscoy/rockpaperscissors/controller) - Manages game logic and event handling.

- [/src/com/aldiyar/rockpaperscissors/model/](https://github.com/Crashjoy/Distributed-Systems-Project/tree/master/src/com/aldiyarscoy/rockpaperscissors/model) - Contains game state and data logic.

- [/src/com/aldiyar/rockpaperscissors/utils/](https://github.com/Crashjoy/Distributed-Systems-Project/tree/master/src/com/aldiyarscoy/rockpaperscissors/utils) - Handles TCP/IP logic.

- [/src/com/aldiyar/rockpaperscissors/view/](https://github.com/Crashjoy/Distributed-Systems-Project/tree/master/src/com/aldiyarscoy/rockpaperscissors/view) - Swing/AWT graphical interface components.

# 📬 Contact
- 💼 Aldiyar Baibogurov
- 📧 abaibogurov@gmail.com
- 🔗 [LinkedIn](https://www.linkedin.com/in/aldiyar-baibogurov/)
!-->
