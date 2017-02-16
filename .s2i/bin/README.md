# angular2-lighttpd

This is an [S2I](https://github.com/openshift/source-to-image) image use to build Angular2 project written in typscript with angular-cli


## Requirements

* [S2I](https://github.com/openshift/source-to-image)
* [Docker](https://www.docker.com/products/docker)


## To build the S2I image

	1. Clone this repository
	2. Execute ```docker build -t angular2-lighttpd .```

## To build an image with your application code

```s2i build git://<source code> angular2-lighttpd <application image>```

## To run your image with Docker

```docker run -it --rm <application image>```

The lighttpd server will listen on port 8080