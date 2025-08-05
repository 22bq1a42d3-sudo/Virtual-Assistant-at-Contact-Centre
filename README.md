# Virtual Assistant - A Multimodal AI Chatbot



<p align="center">
  <strong>An intelligent, locally hosted AI system designed for real-time conversations, voice-controlled interactions, and image-driven understanding.</strong>
</p>

<p align="center">
  Built with next-generation multimodal large language models, this assistant simulates human-like responses for seamless customer engagement and smart task automation.
</p>

---

## 🚀 Features

- **🧠 AI Chatbot**: Powered by LLaMA-3 and LLaVA running locally via Ollama for full privacy.
- **🎤 Voice Interaction**: Full voice command recognition and text-to-speech (TTS) responses.
- **🖼️ Image Understanding**: Accepts image uploads for visual analysis and response generation.
- **📞 Simulated AI Agent**: Can simulate a customer care agent handling phone calls.
- **🔐 Secure Authentication**: Firebase integration for user login and signup.
- **🧍 3D Interaction**: Features a real-time, interactive 3D robot model.
- **🌐 Offline Capable**: Core functionalities work on a local machine without internet access.

---

## 💡 Technologies Used

### 🎨 Frontend Stack
| Tech | Description |
| :--- | :--- |
| **React** | A JavaScript library for building user interfaces. |
| **Three.js** | For rendering and animating the 3D robot model. |
| **Firebase**| Used for authentication (Auth) and database (Firestore). |
| **HTML5/CSS3**| Standard markup and styling for the web interface. |

### 🧠 Backend Stack
| Tech | Description |
| :--- | :--- |
| **Node.js** | A JavaScript runtime for the server-side logic. |
| **Express.js** | A web application framework for Node.js. |
| **Ollama** | For serving LLaMA-3 (text) and LLaVA (vision) models locally. |
| **Firebase Admin** | For secure backend integration with Firebase services. |

---

## 🧱 Project Structure

The project is organized into a frontend application and a backend server.

```bash
virtual-assistant/
│
├── backend/
│   ├── controllers/      # Request handlers
│   ├── routes/           # API routes
│   ├── server.js         # Main server entry point
│   ├── serviceAccountKey.json # Firebase credentials
│   ├── package.json
│   └── package-lock.json
│
├── frontend/
│   ├── public/
│   │   ├── index.html
│   │   └── 019808ab-4e08-7793-90e2-8aeeb0fdefd3.glb # 3D Model
│   │
│   ├── src/
│   │   ├── components/     # Reusable React components
│   │   ├── assets/         # Images, logos, etc.
│   │   ├── App.js
│   │   ├── index.js
│   │   └── firebaseConfig.js # Firebase setup
│   │
│   ├── package.json
│   └── ...
│
├── scripts/
│   ├── setup.sh          # Full setup script for all dependencies
│   └── run_dev.sh        # Script to start both frontend and backend
│
└── README.md
```

---

## 🏁 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

* **Node.js**: Version 18.x or higher.
* **Ollama**: Make sure it is installed and running. You must have pulled the required models:
    ```bash
    ollama pull llama3
    ollama pull llava
    ```
* **Firebase Project**: A configured Firebase project with Authentication and Firestore enabled.
* A modern web browser with support for WebGL for 3D rendering.

### 🔌 Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/virtual-assistant.git](https://github.com/your-username/virtual-assistant.git)
    cd virtual-assistant
    ```

2.  **Backend Setup:**
    * Navigate to the backend directory.
        ```bash
        cd backend
        ```
    * Install dependencies.
        ```bash
        npm install
        ```
    * **Important:** Update `serviceAccountKey.json` with your own Firebase Admin SDK credentials.

3.  **Frontend Setup:**
    * Navigate to the frontend directory.
        ```bash
        cd ../frontend
        ```
    * Install dependencies.
        ```bash
        npm install
        ```
    * **Important:** Configure your Firebase credentials in `src/firebaseConfig.js`.

### ▶️ Running the Application

To run both the frontend and backend servers concurrently, use the provided script from the root directory:
```bash
./scripts/run_dev.sh
```
This will start the backend server (typically on `http://localhost:5000`) and the React frontend development server (typically on `http://localhost:3000`).

---
# Made with love ❤️ by me and my ❤️

## 📄 License

This project is open-source and available under the **MIT License**. See the `LICENSE` file for more details.
