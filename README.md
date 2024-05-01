# http-load-balancer

This project takes advantage of Python3, Flask, Docker, and TDD to demo a HTTP loadbalancer server.

To run the loadbalancer:
> FLASK_APP=loadbalancer.py flask run

Example `curl` request to loadbalancer:
> curl -H 'Host: www.mango.com' 127.0.0.1:5000
{"custom_header":"Test","host_header":"localhost:8082","message":"This is the mango application.","server":"http://localhost:8082/"}
