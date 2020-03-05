# BusyBox with HTTPie-go 

This version of the standard busybox container increases the size a bit (1.2MB to 9.2MB) by adding an HTTPie executable.  (busybox: https://busybox.net/about.html).  In the big scheme of things, this is still a small container.

Thank you to the creators of HTTPie: https://httpie.org/

Thank you to Yusuke Nojima for creating a Go version of HTTPie: https://github.com/nojima/httpie-go

Build instructions for docker:
```
docker build -t <your-username>/busybox:0.1.0 .

# Run the docker container to test it out
docker run -it --rm <your-username>/busybox:0.1.0

# Continue if you want it publicly available..
# (assuming you have a hub.docker.com account and have logged in with 'docker login')

# It's a good idea to have a 'latest' tag too
docker tag <your-username>/busybox:0.1.0 <your-username>/busybox:latest

# push it up to dockerhub.io
docker push <your-username>/busybox:0.1.0
docker push <your-username>/busybox:latest
```
