# Embedded Logging and Simulation System

## Overview
This project showcases the development of an embedded logging mechanism integrated within a codebase to monitor performance and activities. It includes a logging system that captures logs from various processes and sends them to a central server for efficient log management. The project utilizes Linux-based logging mechanisms like syslog and implements fast data transmission using UDP socket programming. With multithreading capabilities through the pthread library and mutexes for optimized log handling, the system ensures real-time client-server interactions and high-performance log processing.

### Key Features

- **Embedded Logging Mechanism:** Developed to be integrated seamlessly within the code, enabling real-time performance tracking and logging of critical events.
- **Linux-Based Log Management:** Utilizes syslog for efficient management and storage of log files, facilitating easier analysis and debugging.
- **Fast Data Transmission:** Implements UDP socket programming for quick data transmission between the client and server, ensuring minimal latency in log delivery.
- **Multithreading and Mutexing:** Employs the pthread library for multithreading, allowing concurrent log processing and handling. Mutexes are used to prevent race conditions, ensuring data integrity and consistent log management.
- **Real-Time Client-Server Interactions:** Designed for real-time interactions between the client and server, enabling immediate response and handling of log data.

### Components

1. **Logger System:** A robust logging system that captures, sends, and manages log messages based on defined severity levels (`DEBUG`, `WARNING`, `ERROR`, `CRITICAL`). The system supports dynamic log level adjustments and efficient log filtering.

2. **Automobile Simulation:** A simulation component that models the behavior of different automobiles in terms of fuel consumption and efficiency. It leverages the logging system to record events such as fuel addition, fuel depletion, and distance driven.

3. **Travel Simulator:** Simulates travel scenarios to test and demonstrate the automobile models' fuel consumption under various conditions. It integrates closely with the logger system to monitor and record the performance and efficiency of each automobile during the simulation. This component offers insights into how different models perform in city versus highway driving conditions, providing valuable data for analysis.

### System Architecture

The system architecture is designed to support high scalability and flexibility, accommodating various logging and simulation scenarios. It incorporates a client-server model for log data transmission, with a focus on low-latency and high-reliability communications. The architecture ensures that log data is processed and stored efficiently, allowing for real-time monitoring and analysis.

### Getting Started

To utilize this system, follow these steps:

- **Clone the Repository:** Start by cloning the project repository to your local machine.
- **Compile the Code:** Use the provided Makefile to compile the source files and generate the executable binaries.
- **Run the Simulations:** Execute the travel simulator to begin the simulation process. The system will automatically start logging events as the simulation progresses.
- **Monitor Logs:** Access the logs on the central server to monitor the simulation's performance and the system's overall health.

### Prerequisites

- Linux operating system with development tools installed.
- Knowledge of C++ programming, especially with regard to network programming and multithreading.
- Familiarity with logging mechanisms and syslog.


