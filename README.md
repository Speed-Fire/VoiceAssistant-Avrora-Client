# Avrora Voice Assistant – Client Application

This repository is part of the **VoiceAssistant Avrora** project group. It contains the **client application** for the Avrora voice assistant.

## Overview

The client is designed to act as the local interface and voice processing unit of the assistant system. It communicates with the central server via **gRPC** and is capable of recognizing voice commands, interacting with the operating system, and controlling external devices.

## Architecture

The application is structured into two main components:

- **Core** – Handles all internal logic, including audio processing, communication with the server, and voice interaction.
- **Interface** – The user-facing component, which connects to the core via a **pipeline** mechanism.

This separation ensures modularity and makes it easier to extend or replace either part independently.

## Key Features

- **Hotword Detection**: Listens for a predefined key phrase to activate the assistant.
- **Voice Recording**: After activation, records the user's speech until silence is detected or a 10-second limit is reached.
- **gRPC Communication**: All interactions with the central server (e.g., command interpretation, data fetching) are performed using gRPC.
- **System Integration**: Can execute actions on the host computer, such as:
  - Launching programs
  - Playing music
  - Other user-defined tasks
- **Device Control**: Supports interaction with **external hardware devices**, enabling smart home or IoT functionality.

## Part of a Bigger System

This client is one of several coordinated components within the **VoiceAssistant Avrora** ecosystem. Other components (such as the server and device controllers) are located in their respective repositories.

## Getting Started

Coming soon...

## License

All rights reserved. 2025
