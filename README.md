# play-framework

Docker image which provides a typesafe activator 1.2.10, designed to launch play applications (v2.3+).

## Run your app

Your play app has to be mounted in the container in the '/app' directory. Should you want to publish your app port to the host, you must use the -p argument.

Here is an example of a docker run command:

```
docker run -d \
  -v /path/to/your/play/app:/app:rw \
  -p 80:9000 \
  ingensi/play-framework
```

## Image inheritance

This docker image inherits from the ingeni/oracle-jdk image. It includes an oracle jdk install in its latest version.
