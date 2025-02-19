# NumPy Calculation Web App

This project is a simple web application that takes user input, processes it using NumPy in a FastAPI backend, and displays the result in a PHP-based frontend.

## Features
- Accepts a list of numbers from the user.
- Uses NumPy to compute the mean of the numbers.
- Displays the result dynamically in a PHP page.
- FastAPI handles backend calculations.
- PHP frontend sends requests to FastAPI.

## Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/Amin-Beep/NumPy.git
cd NumPy
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the FastAPI Server
```bash
uvicorn main:app --reload
```

### 4. Run the PHP Server
```bash
php -S 127.0.0.1:8001
```

### 5. Access the Web App
Open your browser and go to:
```
http://127.0.0.1:8001/index.php
```

## File Structure
```
- main.py (FastAPI backend)
- index.php (PHP frontend)
- requirements.txt (Dependencies for FastAPI)
- README.md (Instructions)
```

## API Endpoint
- **POST /calculate**
  - Accepts: `numbers` (comma-separated string of numbers)
  - Returns: JSON `{ "result": float }`

## Example Usage
1. Enter `10,20,30` in the input field.
2. Click **Calculate**.
3. The result (`20.0`) will be displayed.

## Deployment
You can deploy this project on a cloud service like **AWS or any VPS**. Ensure both FastAPI and PHP run in the same environment.

## License
This project is open-source. Feel free to modify and distribute it.

