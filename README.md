# ros2_docker
This Dockerfile worked on docker on wsl2 on windows11

# build
on wsl2
```bash
xhost local:root
docker build -t ros2:galactic .  
docker run --rm -it --privileged -u ros --net=host -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix ros2:galactic
```

