If you read the source you will see that only the port can be overridden on the command line. If you want to change the host it is served on, you will need to implement the test() method of the SimpleHTTPServer and BaseHTTPServer yourself. But that should be really easy.
And to use it:

> python server.py 127.0.0.1     
Serving HTTP on 127.0.0.1 port 8000 ...

> python server.py 127.0.0.1:9000
Serving HTTP on 127.0.0.1 port 9000 ...

> python server.py 8080          
Serving HTTP on 0.0.0.0 port 8080 ...
