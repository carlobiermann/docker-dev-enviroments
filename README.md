# docker-dev-enviroments


The code in this repository is mainly from Dmitry Danilov's article on [Dockerized build environments for C/C++ projects](https://ddanilov.me/dockerized-cpp-build). 

To build and run the docker container: 
- Make sure to have `docker` installed on your system
- Run
```
$ docker build -t cb_cpp_build_env/cpp_build_env_test:0.1 -f DockerfileCppBuildEnv .
```

