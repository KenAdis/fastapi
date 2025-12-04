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

Install dependencies (recommended in a virtualenv):

```bash
pip install "fastapi[standard]" uvicorn
