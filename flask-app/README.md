# Docker Flask Example

This is a fork of the [Docker Flask example][1] for MLH Localhost Intro
to Docker workshops.

## Running the Example

This example is host on DockerHub as [mlhacks/docker-flask-app][3].  You can download
and run it locally with the following command:

```
$ docker run -p 8888:5000 mlhacks/docker-flask-app
```

## Building the Example

To run this example, you need to build the Docker Image first. To do so, run
the following command:

```
$ docker build -t docker-flask-example .
```

After you've built the image, you can run it as follows:

```
$ docker run -d -p 8888:5000 docker-flask-example
```

The website should now be accessible at [http://localhost:8888/][2].

## License

The original code was released under the Apache License 2.0 by Docker, Inc.
That license is included with this code in the [LICENSE](LICENSE) file.

The modifications to this code are released under the MIT License, copyright 
Major League Hacking, Inc ([READ LICENSE](../README.md)).

[1]: https://github.com/docker/labs/tree/master/beginner/flask-app
[2]: http://localhost:8888
[3]: https://hub.docker.com/r/mlhacks/docker-flask-app/
