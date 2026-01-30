🛡️ CyberNav: Interactive Cybersecurity Roadmap

CyberNav is a comprehensive, interactive single-page application (SPA) designed to guide aspiring cybersecurity professionals. It combines a visual career roadmap with progress tracking, detailed resource curation, and cloud synchronization.

🚀 Key Features

🗺️ Dynamic Career Paths

Switch instantly between four specialized roadmaps:

General Cybersecurity: The foundational baseline (Networking, OS, Scripting).

Red Team (Offensive): Penetration testing, ethical hacking, and evasion.

Blue Team (Defensive): SOC operations, threat hunting, and digital forensics.

GRC: Governance, Risk, and Compliance strategies.

📚 Curated Resource Library

Every learning module includes specific, high-quality links to:

📺 Video Tutorials: (NetworkChuck, Professor Messer, etc.)

⚡ Interactive Labs: (HackTheBox, TryHackMe, OverTheWire)

📄 Documentation: (NIST, OWASP, Microsoft Learn)

☁️ Cloud Sync & Tracking

Google Authentication: Integrated via Firebase to save progress across devices.

Visual Analytics: Real-time Chart.js visualizations of your Skill Gap (Radar Chart) and Phase Completion (Bar Chart).

Guest Mode: Fully functional offline mode using local browser storage.

🎨 Modern UI/UX

Sticky Information Panel: Reference learning materials while scrolling the roadmap.

Responsive Design: Optimized for Desktop (Sticky Layout) and Mobile (Scrollable).

Dark/Light Mode Elements: Professional aesthetic using Tailwind CSS.

🛠️ Technology Stack

Frontend: HTML5, Vanilla JavaScript (ES6+)

Styling: Tailwind CSS (via CDN)

Visualization: Chart.js (via CDN)

Backend: Google Firebase v11 (Authentication & Firestore)

Icons: Unicode & SVGs

📦 Installation & Setup

Since this is a Single-File Application, setup is instant.

Download the Code:
Download the Cybersecurity_Roadmap_Production.html file (rename it to index.html for hosting).

Run Locally:
Simply double-click the file to open it in Chrome, Firefox, or Edge.

Deploy (Optional):
Upload the file to GitHub Pages, Netlify, or Vercel for free hosting.

⚙️ Configuration (Firebase)

The application is currently pre-configured with Firebase credentials. If you wish to host this yourself using your own database:

Go to the Firebase Console.

Create a new project.

Enable Authentication:

Go to Build > Authentication > Sign-in method.

Enable Google.

Enable Database:

Go to Build > Firestore Database.

Create Database (Start in Test Mode).

Update Code:

Open index.html in a text editor.

Scroll to the bottom <script type="module"> section.

Replace the firebaseConfig object with your own keys:

const firebaseConfig = {
    apiKey: "YOUR_NEW_API_KEY",
    authDomain: "your-project.firebaseapp.com",
    projectId: "your-project-id",
    storageBucket: "your-project.firebasestorage.app",
    messagingSenderId: "SENDER_ID",
    appId: "APP_ID",
    measurementId: "G-MEASUREMENT_ID"
};


🖥️ Usage Guide

Choose Your Role: Use the top bar to select your career path (e.g., "Red Team").

Explore Modules: Click on any node in the timeline on the left.

Learn: The right-hand panel will lock in place and show you specific videos and labs for that topic.

Login: Click the "Login" button in the top right to enable cloud saving.

Track: Check the boxes as you complete skills. Your "XP" and graphs will update automatically in the Dashboard view.

🤝 Contributing

Contributions are welcome! If you have better resources (YouTube links, free labs) to add to the roadmapData object in the code:

Fork the repository.

Edit the roadmapData array in the JavaScript section.

Submit a Pull Request.

📄 License

This project is licensed under the MIT License - free to use and modify.
