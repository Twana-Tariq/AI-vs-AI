# AI-vs-AI
Building an Intelligent Detecter Against “Made Up” Content
With the continuous evolution of Artificial Intelligence, distinguishing between real and AI generated content has been a challenge. This project has a detection system with the capability of distinguishing whether a certain image, audio, video, or a live broadcast has been altered or generated by AI.

## Goal
We aim to develop a system that can flag a wide range of content such as image, audio, video, and live broadcasts. We also intend on making our system scalable to ensure we can keep up with AI’s evolution.

### Repositry Structre 
AI-vs-AI/
├─ backend/               # Contains the server code and AI detection logic
├─ frontend/              # Contains the web interface (user dashboard)
├─ detection_engine/      # Holds AI models for text, image, audio, video detection
├─ docs/                  # Project reports, documentation, and presentations
├─ database/              # Database schemas and configuration files
├─ scripts/               # Automation or testing scripts
├─ tests/                 # Test files to verify code functionality
├─ .gitignore             # Files Git should ignore (e.g., node_modules, .env)
├─ LICENSE                # Project license information
└─ README.md              # This file

Each folder in the repository has a specific purpose:
backend/ → where the detection logic and APIs live.
frontend/ → user interface for uploading and checking content.
detection_engine/ → model training and evaluation code.
docs/ → project proposal, report, and related materials.
database/ → SQL or NoSQL configuration for saving detection results.
scripts/ → helpful utilities like setup or testing scripts.
tests/ → automated test cases to ensure functionality.
