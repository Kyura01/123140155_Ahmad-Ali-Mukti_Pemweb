# Pyramid Web Application with Waitress

A simple Pyramid web application demonstrating basic web server setup using Waitress as the WSGI server.

## Features

- **Simple configuration and startup process**
- **Uses Waitress as WSGI server**
- **Basic view function returns HTML response**
- **Shows Pyramid's minimal setup requirements**

## Installation

1. Install required dependencies:
```bash
pip install pyramid waitress
```

## Usage

Run the application:
```bash
python App.py
```

The server will start on `http://0.0.0.0:6543` and display "Hello World!" when accessed.

## Code Structure

- Simple view function that returns an HTML response
- Pyramid configurator setup with routing
- Waitress WSGI server for production-ready serving
- Minimal boilerplate for quick development

## Extra Credit Answers

### Print statement differences:

- **Parentheses version is Python 3 syntax**
- **Without parentheses is Python 2 legacy syntax**

### Return value alternatives:

- **HTML string requires Response() wrapper**
- **Integer sequences aren't valid responses**

### Invalid code impacts:

- **NameError shows error handling**
- **Demonstrates debugging capabilities**

### WSGI's heritage:

- **Based on CGI standard**
- **Standardizes web server/app interface**

## Technical Notes

This application demonstrates:
- Pyramid framework's minimal setup requirements
- WSGI server integration with Waitress
- Basic HTTP request/response handling
- Production-ready server configuration