# Understanding API Authentication (Node.js + Express + Axios + Postman)

- Description:
  - This project demonstrates various API authentication methods using a Node.js and Express backend.
  - It interacts with the Secrets API (App Brewery) to show how to securely access data using different authentication strategies.
  - Implemented using Axios for API calls, EJS for rendering, and Postman for testing all routes.

# Technologies Used
- Node.js – JavaScript runtime environment
- Express.js – Web framework for handling routes
- Axios – For making HTTP requests
- body-parser – Middleware for parsing request data
- EJS – Template engine for rendering responses
- Postman – API testing and debugging tool
- HTML / CSS – For front-end layout and styling

# Project Summary
- The app connects to the Secrets API to fetch and display secret data using four authentication types:
  - No Authentication – Access public data (/random)
  - Basic Authentication – Username and password-based access (/all?page=2)
  - API Key Authentication – Using an API key as a query parameter (/filter)
  - Bearer Token Authentication – Using a token in the request header (/secrets/:id)
- Each response is rendered dynamically in the EJS template as formatted JSON.

# Features
- Demonstrates 4 major API authentication techniques
- Clean implementation using Express and Axios
- Tested thoroughly using Postman
- Dynamically displays API responses in the browser
- Beginner-friendly and educational
- Runs locally on port 3001

# How to Use
- Clone the Repository:
  - ```bash
    git clone https://github.com/Rudhar-cmd/API-Authentication-Demo.git
    ```
- Navigate into the Project Folder:
  - ```bash
    cd API-Authentication-Demo
    ```
- Install Dependencies:
  - ```bash
    npm install
    ```
- Start the Server:
  - ```bash
    node index.js
    ```
- Open in Browser:
  - Visit: http://localhost:3001
- Available Routes:
  - /noAuth → Access public data  
  - /basicAuth → Use Basic Authentication  
  - /apiKey → Use API Key Authentication  
  - /bearerToken → Use Bearer Token Authentication  

# Postman Testing Guide
- GET /noAuth → No authentication required  
  - URL: http://localhost:3001/noAuth
- GET /basicAuth → Set Basic Auth in Postman  
  - Username: Rudhar_35  
  - Password: XXXX
- GET /apiKey → Add query parameter  
  - Key: apiKey  
  - Value: XXXX
- GET /bearerToken → In Headers, add  
  - Key: Authorization  
  - Value: Bearer XXXX
- Observe JSON responses in Postman or in your browser.

# Folder Structure
- public/ → Static assets like CSS  
- views/ → EJS templates (index.ejs)  
- index.js → Main server file with all routes and authentication logic  

# Example Credentials
- Username: Rudhar_35  
- Password: XXXX  
- API Key: XXXX  
- Bearer Token: XXXX  

# License
- This project is open source and available under the MIT License.
