# SETUP AND RUN GUIDE

This guide provides complete step-by-step instructions for running the entire application, including backend setup, mobile app setup, running instructions, Docker setup, API testing, and troubleshooting.

## Table of Contents
1. [Backend Setup](#backend-setup)
2. [Mobile App Setup](#mobile-app-setup)
3. [Running Instructions](#running-instructions)
4. [Docker Setup](#docker-setup)
5. [API Testing](#api-testing)
6. [Troubleshooting](#troubleshooting)

---

## Backend Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/princeQ85/quick-commerce-platform.git
   cd quick-commerce-platform
   ```
2. Install the required dependencies:
   ```bash
   npm install
   ```
3. Set up the environment variables. Create a `.env` file based on `.env.example`:
   ```bash
   cp .env.example .env
   ```
4. Run the backend server:
   ```bash
   npm start
   ```

## Mobile App Setup
1. Navigate to the mobile app directory:
   ```bash
   cd mobile-app
   ```
2. Install the dependencies:
   ```bash
   npm install
   ```
3. Start the mobile app:
   ```bash
   npm start
   ```
   You can also run it on an emulator or a physical device.

## Running Instructions
- Make sure the backend server is running before starting the mobile app.
- You may access the app on `http://localhost:3000`.

## Docker Setup
1. Ensure Docker is installed on your machine.
2. Build the Docker image:
   ```bash
   docker build -t quick-commerce-platform .
   ```
3. Run the Docker container:
   ```bash
   docker run -p 3000:3000 quick-commerce-platform
   ```

## API Testing
1. Use tools like Postman or curl to test the API endpoints.
2. Ensure the backend server is running.
3. Example of an API request:
   ```bash
   curl http://localhost:3000/api/v1/products
   ```

## Troubleshooting
- If you encounter issues:
  - Check if all services are running.
  - Look for error messages in the console.
  - Ensure that the ports are not being used by another application.
  - Review the `.env` configuration for errors.

If you continue to face issues, please refer to the documentation or seek help in the GitHub repository's issues section.