# docker-dev-enviroments


The code in this repository is mainly from Dmitry Danilov's article on [Dockerized build environments for C/C++ projects](https://ddanilov.me/dockerized-cpp-build)


1. Download this repository:
```
$ git clone git@github.com:carlobiermann/docker-dev-enviroments.git
```

2. Build the docker container: 
- Make sure to have `docker` installed on your system
- Run
```
$ cd cpp-dev-env/docker-files/
$ docker build -t cb_cpp_build_env/cpp_build_env_test:0.1 -f DockerfileCppBuildEnv .
```

3. Run the docker container: 
```
$ cd ../../
$ docker run -it --rm --name=example_container \
	--mount type=bind,source=${PWD},target=/src \ # Mount the current directory
	example/example_build:0.1 \
	bash
```
