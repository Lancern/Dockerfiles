# Tuna

This docker image provides a base image with `apt` source replaced by TUNA. Consumers of this image should use it as a base image of their images.

Before running `apt-get` in your image, please ensure that the local `apt` cache is properly updated:

```dockerfile
RUN apt-get --assume-yes update
```
