# flask
A Python Flask Docker Image.

This is an implementation of the GCP [Quickstart Image](https://cloud.google.com/container-registry/docs/quickstart).
The image is stored in Docker Hub instead of the GCP container registry.

## Run the image:
```
$ docker run -d -p 80:80 --name flask danehans/flask:latest
```

## (Optional) Instead of running the pre-built image, you can build the image:
```
$ docker build -t flask .
```

## Test the running container:
```
$ curl http://localhost
<h3>Hello, World!</h3>
```

## Remove the container:
```
$ docker rm -f flask
```