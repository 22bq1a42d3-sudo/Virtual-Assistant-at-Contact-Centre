An intelligent, locally hosted AI system designed for real-time conversations, voice-controlled interactions, and image-driven understanding.

Built with next-generation multimodal large language models, this assistant simulates human-like responses for seamless customer engagement and smart task automation.

🚀 Features
🧠 AI Chatbot powered by LLaMA3 & LLaVA (via Ollama)
🎤 Voice command recognition
🖼 Image input and visual response generation
📞 Simulated AI phone call handling (Customer Care Agent)
🔐 Firebase Authentication (Login/Signup)
🧍 Real-time 3D Robot Model interaction
🌐 Works offline on local machine
🧱 Project Structure
virtual-assistant/
│
├── frontend/
│ ├── src/
│ ├── 019808ab-4e08-7793-90e2-8aeeb0fdefd3.glb # 3D Robot Model
│ ├── App.css
│ ├── App.js
│ ├── App.test.js
│ ├── background.webp
│ ├── index.css
│ ├── index.html
│ ├── index.js
│ ├── login.html
│ ├── logo.svg
│ ├── profile.html
│ ├── reportWebVitals.js
│ └── setupTests.js
│
├── backend/
│ ├── controllers/
│ ├── routes/
│ ├── server.js
│ ├── serviceAccountKey.json.json
│ ├── package.json
│ └── package-lock.json 
💡 Technologies Used
🎨 Frontend Stack
HTML5
HTML5	CSS3
CSS3	JavaScript
JavaScript	React
React	Three.js
Three.js	Firebase Auth
Firebase Auth	Firestore
Firestore
🧠 Backend Stack
Node.js
Node.js	Express.js
Express.js	Firebase Admin
Firebase Admin	LLaMA 3
LLaMA 3	LLaVA
Prerequisites
Node.js ≥ 18
Ollama (LLaMA 3 & LLaVA models pulled)
Firebase project set up
GLB-supported 3D rendering enabled in browser
🔌 Backend Setup
cd backend
npm install
node server.js
Update serviceAccountKey.json.json with your Firebase Admin credentials.

🌐 Frontend Setup
cd frontend# If using Create React App
npm install
npm start
📚 Topics & Tags
Chatbot Voice Commands Image Processing NLP Machine Learning LLM Training Firebase Ollama LLaMA 3 LLaVA

🙋‍♂ Author
Author Avatar	Seelam Abhinav
Student @ VVIT
GitHub Profile
📄 License
This project is open-source and available under the MIT License.
