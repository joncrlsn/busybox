# BusyBox with HTTPie-go 

This version of the standard busybox container increases the size a bit by adding an HTTPie implementation.  https://hub.docker.com/\_/busybox  (busybox: https://busybox.net/about.html)

Thank you to the creators of HTTPie: https://httpie.org/

Thank you to Yusuke Nojima for creating a Go version of HTTPie: https://github.com/nojima/httpie-go

Build instructions:
```
docker build -t <your-username>/busybox:0.1.0 .

# It's a good idea to have a latest tag too
docker tag <your-username>/busybox:0.1.0 <your-username>/busybox:latest

# Assuming you have a dockerhub.io account and have logged in with 'docker login'
docker push <your-username>/busybox:0.1.0
docker push <your-username>/busybox:latest
```
