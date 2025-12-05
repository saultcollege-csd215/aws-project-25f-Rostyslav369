
In this project, NGINX is used as a reverse proxy in front of the Flask app on the EC2 instance. The Flask app runs on a private port (port 8000), and NGINX listens on the public web port (port 80). When a user opens the EC2 public IP in a browser, NGINX receives the request and sends it to the Flask app.

The main purpose of using NGINX as a reverse proxy is security. The Flask app is not directly exposed to the internet. Only NGINX is public, which makes the system safer.

Another benefit is performance. NGINX is very fast at handling web requests and makes the Flask app run more smoothly.

Using a reverse proxy also makes the project more realistic and closer to how real web servers are deployed in production.
