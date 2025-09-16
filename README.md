# Sentinnel-Connect
Sentinel Connect is a military-grade secure communications platform that enables encrypted messaging, emergency coordination, family connectivity, and professional training resources. It is designed for field agents, command centers, and their families to stay connected while maintaining top-level security and confidentiality.

Overview

Sentinel Connect is designed to be used in sensitive environments where confidentiality, integrity, and availability are required. 
The system separates responsibilities between front-end clients, back-end services, and persistent storage, and enforces security at every layer.

Features

End-to-end encrypted messaging for one-to-one and group conversations<br>
Secure family portal for non-operational updates and scheduled video calls<br>
Emergency services module with verified contacts and location-aware support<br>
Training hub for mission-critical courses, materials, and certifications<br>
Role-based access control with security classifications: Unclassified, Secret, Top-Secret<br><br><br>

Tech stack<br>

Frontend: React.js and Tailwind CSS<br>
Backend: Node.js with Express framework<br>
Database: MongoDB or PostgreSQL (configurable based on operational needs)<br>
Security: TLS/HTTPS for transport, AES-256 for data encryption at rest, and secure key management<br>
Authentication: JWT (JSON Web Tokens) and role-based authorization<br>

Setup and installation<br><br>
Clone the repository<br>

Clone the repository:
```bash
git clone https://github.com/Nidhi-hb/Sentinnel-Connect.git
```
Move to the file
```bash
cd Sentinnel-Connect
```
Install dependencies for the server and client (if separate)
```bash
npm install
```
Create a configuration file named .env in the project root with the following variables:
```bash
PORT=3000
DB_URI=your_database_connection_string
JWT_SECRET=your_jwt_secret
ENCRYPTION_KEY=your_256bit_encryption_key
```
Start the development server
```bash
npm run dev
```
Open the application in your browser at https://localhost:3000 or the configured host and port<br><br>

Project Structure 
```bash
sentinel-connect/
├─ client/         # Frontend React app
├─ server/         # Backend Express API
├─ public/         # Static assets
└─ README.md
```
<br>

Security considerations<br><br>

Always run the service behind a TLS-terminating reverse proxy or load balancer<br>
Use hardware security modules or cloud key management for storing encryption keys<br>
Enable audit logging to capture critical operations and access events<br>
Apply role-based access control consistently across APIs and UI components<br>
Use multi-factor authentication for administrative accounts<br>

Directory layout<br><br>

client - front-end application code<br>
server - back-end APIs, authentication, and encryption logic<br>
scripts - automation and deployment scripts<br>
public - public assets and static files<br>


Create a feature branch for each change<br>
git checkout -b feature/short-description

Make changes and run tests locally<br>
npm test<br>

Commit with a clear message
```bash
git add . git commit -m "short, descriptive message"
```
Push the branch and open a pull request for review
```bash
git push origin feature/short-description
```

Deployments

Containerize the server using Docker and follow your organization's CI/CD pipeline
Ensure environment variables are supplied securely by the deployment system
Configure scalable database and storage options appropriate for load
Monitor application health and set up alerts for critical metrics

<p align="center">
  <img src="images/s1.png" alt="Screenshot 1" width="600" height="340">
</p>

<p align="center">
  <img src="images/s2.png" alt="Screenshot 2" width="600" height="340">
</p>

<p align="center">
  <img src="images/s3.png" alt="Screenshot 3" width="600" height="340">
</p>
