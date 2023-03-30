# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:

### STEP 2:

### STEP 3:

Write your own steps

## PROGRAM
```python
from http.server import HTTPServer,BaseHTTPRequestHandler

content='''
<!doctype html>
<html>
<head>
<title> My Web Server</title>
</head>
<body>
<h1>Top Five Web Application Development Frameworks</h1>
<h2>1. Django</h2>
<h2>2. MEAN Stack</h2>
<h2>3. React </h2>
<h2>4. MERN</h2>
<h2>5. Spring Framework</h2>
</body>
</html>
'''

class MyServer(BaseHTTPRequestHandler):
    def do_GET(self):
        print("Get request received...")
        self.send_response(200) 
        self.send_header("content-type", "text/html")       
        self.end_headers()
        self.wfile.write(content.encode())

print("This is my webserver") 
server_address =('',8000)
httpd = HTTPServer(server_address,MyServer)
httpd.serve_forever()
```
## OUTPUT
### Server Output:
![w2](https://user-images.githubusercontent.com/117974950/228801020-08db6e2f-c2b4-4f8a-bfab-f43034494f67.png)

### Client Output:
![clientop](https://user-images.githubusercontent.com/117974950/228801142-145a37c7-ce98-41ea-963b-8c0eb62b5ad4.png)

## RESULT
The program is executed succesfully
