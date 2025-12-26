# Currency API Client

## Project Description
This project is a **command-line API client** written in Python that interacts with a public currency exchange rate API.
It allows users to:

- Fetch latest currency exchange rates
- Convert an amount from one currency to another

The project uses a simple CLI interface and demonstrates how to consume REST APIs using Python.

---

##  Purpose of the Project
This project is:
-  A learning exercise
-  A simple API client
-  Not a production-ready financial tool

It is designed to practice:
- API requests
- Command-line argument handling
- Basic error handling

---

##  Tech Stack
- **Language:** Python
- **Library:** requests
- **Execution:** Command Line (CLI)
- **Data Format:** JSON
- **External API:** Exchange Rates API

---

##  How the Code Works
- The script reads an optional `config.json` file to get the API base URL
- If `config.json` is not present, a default API URL is used
- API requests are made using the `requests` library
- Responses are parsed as JSON
- Errors are handled using try–except blocks
- Command-line arguments determine the action to perform

---

 Project Files
project/
│

├── client.py # Main API client script

├── config.json # (Optional) API base URL configuration

├── README.md # Project documentation

---

## ⚙️ Installation Steps

1. Clone the repository:
git clone <repository-url>

   cd project
   
3. (Optional) Create a virtual environment:

   python -m venv venv

4. Activate the virtual environment:

   venv\Scripts\activate

5. Install required dependency:

   pip install requests

 Command-Line Usage

The script supports two commands: rates and convert.

 Fetch Currency Rates

 python client.py rates --from USD

 Convert Currency

 python client.py convert --from USD --to INR --amount 10

Example Output

Rates Output
{
  "base_code": "USD",
  "rates": {
    "INR": 83.2,
    "EUR": 0.92
  }
}

Convert Output

10 USD = 832.0 INR

Error Handling

Handles network and API errors gracefully

Prints meaningful error messages for:

Invalid currencies

Missing arguments

API request failures

Limitations

No automated tests included

No authentication handling

Uses a public API without rate-limit handling

Conclusion

This project demonstrates how to build a simple CLI-based API client in Python.

It is suitable for learning API consumption, CLI argument parsing, and basic error handling.
