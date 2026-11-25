# To run the previous just use 
```bash
docker build -t multi:full -f Dockerfile-old .
```
It creates the slim image of the compiled server and client go app.
But you can also do it with the multi target build, that creates the specified image.
```bash
docker build -t multi:client --target prod-client -f ockerfile-final .
# and
docker build -t multi:server --target prod-server -f Dockerfile-final .
```
