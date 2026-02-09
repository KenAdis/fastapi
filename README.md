# Simple FastAPI Todo API

This repository contains a minimal **FastAPI** application that exposes a basic in-memory **Todo list** API.  
All logic lives in `main.py`.

## Features

- In-memory todo storage (no database)
- Pydantic models for request/response validation
- Enum-based priority field (`LOW`, `MEDIUM`, `HIGH`)
- CRUD-style endpoints:
  - Get a single todo
  - Get a list of todos
  - Create a new todo
  - Update an existing todo
  - Delete a todo

## Requirements

- Python 3.10+
- FastAPI
- Uvicorn

## How to Run `main.py`

From the directory containing `main.py`, run the following commands **in order**.

```bash
# 1. Create a virtual environment
python3 -m venv venv

# 2. Activate the virtual environment
source venv/bin/activate

# 3. Install dependencies
pip install "fastapi[standard]" uvicorn

# 4. Run the FastAPI application
uvicorn main:api --reload
