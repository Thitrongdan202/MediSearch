# MedicineSearch

## Installation Guide

### 1. Create and Activate a Python Virtual Environment

Make sure Python 3.13 is installed on your system.

Create a virtual environment:

```bash
python3.13 -m venv venv
```

Activate the virtual environment:

On macOS/Linux:

```bash
source venv/bin/activate
```

On Windows:

```bash
venv\Scripts\activate
```

### 2. Install the Required Dependencies

Install all required packages from the `requirements.txt` file:

```bash
pip install -r requirements.txt
```

### 3. Configure Environment Variables

Create a `.env` file in the project root directory and add your Gemini API key:

```env
GEMINI_KEY="YOUR_GEMINI_API_KEY"
```

### 4. Apply Database Migrations

Run the following command to initialize and update the database:

```bash
python manage.py migrate
```

### 5. Vectorize the Dataset

Run the following command to process and vectorize the medical dataset:

```bash
python vectorize.py
```

### 6. Run the Application

Start the Django development server:

```bash
python manage.py runserver
```

Open the following URL in your browser:

```text
http://127.0.0.1:8000/search/
```
