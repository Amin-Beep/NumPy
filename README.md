# NumPy

NumPy Calculation Web App

This project is a simple web application that takes user input, processes it using NumPy in a FastAPI backend, and displays the result in a PHP-based frontend.

Features

Accepts a list of numbers from the user.

Uses NumPy to compute the mean of the numbers.

Displays the result dynamically in a PHP page.

FastAPI handles backend calculations.

PHP frontend sends requests to FastAPI.

Installation & Setup

1. Clone the Repository

git clone https://github.com/Amin-Beep/NumPy-CBMI.git
cd NumPy-CBMI

2. Install Dependencies

pip install -r requirements.txt

3. Run the FastAPI Server

uvicorn main:app --reload

4. Run the PHP Server

php -S 127.0.0.1:8001

5. Access the Web App

Open your browser and go to:

http://127.0.0.1:8001/index.php

File Structure

- main.py (FastAPI backend)
- index.php (PHP frontend)
- requirements.txt (Dependencies for FastAPI)
- README.md (Instructions)

API Endpoint

POST /calculate

Accepts: numbers (comma-separated string of numbers)

Returns: JSON { "result": float }

Example Usage

Enter 10,20,30 in the input field.

Click Calculate.

The result (20.0) will be displayed.

Deployment

You can deploy this project on a cloud service like Heroku, Vercel, or a VPS. Ensure both FastAPI and PHP run in the same environment.

License

This project is open-source. Feel free to modify and distribute it.

