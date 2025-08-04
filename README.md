# Robot Compost Control Panel Backend

## 📄 Introduction

This repository contains the Express.js backend server for the robot compost system. It is responsible for handling API requests from the frontend, processing data, and managing communication with the Raspberry Pi controller.

### 💻 Technologies Used

- **Express.js & Node.js:** The core framework for building the backend API.
- **MySQL:** A database for storing and retrieving sensor data.
- **AWS Services:** Hosted on AWS Lambda with an API Gateway endpoint.

## 🚀 Getting Started

### 📝 Prerequisites

-   **Node.js**: Version **v22.14.0** or later.
-   **npm**: For package management.
-   **MySQL Database:** An instance of MySQL running locally or remotely.
-   **Raspberry Pi:** A physical Raspberry Pi computer is required for the full system.

### 📦 Installation

1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/Marcuswzh/Control_panel_backend.git](https://github.com/Marcuswzh/Control_panel_backend.git)
    cd Control_panel_backend
    ```

2.  **Install dependencies:**
    ```sh
    npm install
    ```

### ⚙️ Configuration

-   **Environment Variables:** This backend requires sensitive configuration details, such as database credentials and AWS API keys. These were stored in a `.env` file, which is not committed to the repository for security.
-   **Lab-Specific Details:** Crucial information, including **MySQL database credentials, AWS API keys, and MQTT broker details**, are recorded on the physical whiteboard in the lab. The next batch of interns must use this information to set up their `.env` file and configure their AWS services.
-   **Essential Files:** Note that `script.js` is an essential part of the backend logic but is not a script to be run directly.

### ▶️ Running the Application

1.  **Start the Backend Server:**
    ```sh
    node server.js
    ```

### 🤖 Raspberry Pi Python Code

> **Important:** The Python code for the Raspberry Pi controller is **not** included in this repository. It is located on the physical Raspberry Pi computer in the lab. To find the command, just arrow key up till you
> see the following below:

-   **Code Location:** The Python files are stored at the following path on the Raspberry Pi:
    `/home/globalpbl2425/PBL2425/`
-   **Dependencies:** The Python dependencies must be installed in a virtual environment (`.venv`).
-   **Running the Script:** To run the main Python controller script, use the following command:
    ```sh
    /home/globalpbl2425/PBL2425/.venv/bin/python /home/globalpbl2425/PBL2425/__init__v3.py
    ``'
