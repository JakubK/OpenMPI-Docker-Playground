## OpenMPI Docker Playground

Simple docker-compose script I made to quickly set up my development environment for "High performance computing systems" subject on Gdansk University of Technology.

It makes use of <a href="https://hub.docker.com/r/mfisherman/openmpi">mfisherman/openmpi</a> docker container having all the dependencies installed.

### How to use

Move your C program file named as `program.c` to `project` directory and run

```sh
docker-compose up
```

The output of your program should be printed out making container exit. 

Mentioned `project` directory already contains example `program.c` file.\
From that directory you can modify the `program.c` however you like and re-run the mentioned command to see the new results.