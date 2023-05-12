## OpenMPI Docker Playground

Simple docker-compose script I made to quickly set up my development environment for "High performance computing systems" subject on Gdansk University of Technology.

It makes use of <a href="https://hub.docker.com/r/mfisherman/openmpi">mfisherman/openmpi</a> and <a href="https://hub.docker.com/r/mfisherman/openmp">mfisherman/openmp</a> docker containers having all the dependencies installed.

### How to use

Move your C program file named as `program.c` to `project` directory and run

```sh
docker-compose up <service_name>
```

service_name one of the following:

- openmpi - Starts container with openmpi and make installed, need to get into it and execute everything by yourself

- openmpiff - Starts container and runs the hardcoded OpenMPI compilation and run process and then exits 

- openmp - Starts container with openmp and make installed, need to get into it and execute everything by yourself


Mentioned `project` directory already contains example `program.c` file.\
From that directory you can modify the `program.c` however you like and re-run the mentioned command to see the new results.