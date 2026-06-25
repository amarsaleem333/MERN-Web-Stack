# MERN Web Stack Deployment on AWS Cloud

This project guides you through implementing a complete web solution based on the **MERN (MongoDB, Express, React, Node.js)** stack deployed in the AWS Cloud environment.

---

## 🛠️ Project Architecture

The MERN Web stack consists of the following architectural components:
* **MongoDB:** A document-based, No-SQL database used to store application data in the form of flexible documents.
* **ExpressJS:** A minimalist, server-side web application framework running on top of Node.js.
* **ReactJS:** A modern frontend framework developed by Facebook, used for building reactive User Interfaces (UI) in the browser.
* **Node.js:** A JavaScript runtime environment that executes JavaScript code outside of a browser.

---

## 🚀 Deployment Steps

### Step 1: AWS Provisioning & Instance Configuration
1. Log into your AWS Console and launch an **Ubuntu Server LTS** EC2 instance (`t2.micro`).
2. Configure your Security Groups (`launch-wizard-1`) to allow inbound traffic on the following critical ports:
   * **Port 22 (SSH):** Remote access management.
   * **Port 3000:** Custom TCP for the frontend React development server.
   * **Port 5000:** Custom TCP for the backend Node.js server (if applicable).

### Step 2: Backend Development & Node.js Setup
1. Update and upgrade Ubuntu's package manager:
   ```bash
   sudo apt update && sudo apt upgrade -y

________________________________________________________________________________________________________________

Locate and install Node.js on your server from the Ubuntu repositories or Nodesource.

Initialize your project directory and configure the Express server, setting up models, routes, and controllers for your Todo application.

Step 3: MongoDB Database Integration
Leverage a cloud-managed database solution (e.g., MongoDB Atlas) to handle your application records securely.

Ensure you whitelist your EC2 instance's IP address or allow global network access (0.0.0.0/0) during initial staging to permit incoming DB requests.

Securely pass your MongoDB connection string (DB) to your Node.js application environment files.

Step 4: Frontend Development (ReactJS)
In the root Todo directory, generate your React boilerplate using:

Bash
npx create-react-app client
Customize the frontend layout. Update your CSS layout elements in src/index.css or src/App.css to build a clean responsive user experience.

Bash
vim src/index.css
Ensure components match requirements for a seamless user feedback loop to the backend API.

Step 5: Application Execution & Verification
Navigate back to your core project directory:

Bash
cd ../..
Launch the server application stack using the runtime pipeline configuration scripts:

Bash
npm run dev
📸 Deployment Evidence & Verification
Below are verified structural captures demonstrating successful server configuration, code setup, and application execution:

📡 AWS Security Group Matrix
Verify that your inbound/outbound rules match the required mapping for port 3000 and 22:

💻 Backend Core Execution
📁 Application Routing & Database Connection
⚡ React Components & API Aggregation

---






_______________________________
