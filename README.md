# FastHttpServer - Simple, Lightweight, and Fast HTTP Server

## Overview

**FastHttpServer** is a pip package that offers a simple, lightweight, and fast HTTP server implemented in Python. This server provides a minimalistic solution for serving static content and handling basic HTTP requests. It is designed to be easy to set up, efficient in serving web content, and accessible as a pip-installable package.

## Installation

To install FastHttpServer, use the following pip command:

```bash
pip install FastHttpServer
```

Also make sure the python 'socket' package is installed


## Usage

1. After installation, you can import the package:


```python
import FastHttpServer
```

2. To run the server use the initServer() function and specify the port:


```python
FastHttpServer.initServer(3000)
```

This will make the server listen on `localhost` at port `3000`. You can customize the port by changing the port parameter.


3. Access the server in your browser:

Open your web browser and navigate to [http://localhost:3000](http://localhost:3000) (or the custom port you specified). You should see a 404 page indicating that the server is running.

4. Specify the routes of the server

use the route wrapper and specify the route path. Make sure the proceeding function has a request parameter:

```python
@FastHttpServer.route('/')
def index(request):
    return '<h1>Success!</h1>'
```

## Notes

- This server is suitable for serving static content in development and testing environments. For production use, consider security and scalability aspects.

- FastHttpServer is intentionally kept minimalistic. For more advanced features and dynamic content, consider using a full-fledged web framework.

Feel free to use and contribute to FastHttpServer. Keep your web serving simple and enjoy the speed!