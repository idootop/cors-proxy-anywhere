# cors-proxy-anywhere

Use Nginx and Docker to create a reverse proxy that addresses CORS issues during local development.

## ⚡️ Get Started

```shell
# Create a CORS proxy from https://google.com to http://localhost:3000
docker run -d \
    -e TARGET=https://google.com \
    -p 3000:80 \
    idootop/cors-proxy-anywhere:1.0.0

# Create a CORS proxy from http://localhost:3000 to http://localhost:3001
docker run -d \
    -e TARGET=http://host.docker.internal:3000 \
    -p 3001:80 \
    idootop/cors-proxy-anywhere:1.0.0
```
