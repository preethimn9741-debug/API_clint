# API Client

## 📌 Project Description
**API Client** is a Python-based command-line tool that interacts with REST APIs.
It sends HTTP requests (GET, POST, PUT, DELETE), handles responses, and displays or saves results in a structured format.

This project is created as a **learning and practice project** to understand how client-side applications communicate with APIs.

---

## 🎯 Purpose of the Project
This project is:
- ✅ A learning exercise  
- ✅ A reusable API client utility  
- ❌ Not a production-ready client library  

It helps in understanding API consumption, request handling, and response processing.

---

## ✨ Features
- Send HTTP requests to REST APIs
- Supports GET, POST, PUT, and DELETE methods
- Handles JSON request and response data
- Displays API responses in readable format
- Supports command-line execution
- Basic error handling for failed requests

---

## 🛠 Tech Stack
- **Language:** Python  
- **Library:** requests  
- **Execution:** Command Line (CLI)  
- **Data Format:** JSON  

---

## 🏗 Architecture Overview
- The client sends HTTP requests using the `requests` library
- API responses are parsed as JSON
- Errors such as invalid URLs or failed requests are handled gracefully
- Output can be printed to the console or saved for later use

---

## 📂 Project Structure
api_client/
│
├── api_client.py # Main API client script
├── requirements.txt # Python dependencies
├── README.md # Project documentation\

---

## ⚙️ Installation Steps

1. Clone the repository:
```bash
git clone <repository-url>
cd api_client
1 (Optional) Create a virtual environment:
         python -m venv venv
2 Activate the virtual environment:
         venv\Scripts\activate
3 Install dependencies:
         pip install -r requirements.txt
4 Run the API Client
         python api_client.py
Example Output
{
  "userId": 1,
  "id": 1,
  "title": "Sample title",
  "body": "Sample body"
}

