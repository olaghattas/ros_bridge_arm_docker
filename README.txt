 Installing the following packages should allow you to enable support for aarch64 containers on your x86 workstation:
   sudo apt-get install qemu binfmt-support qemu-user-static # Install the qemu packages
   docker run --rm --privileged multiarch/qemu-user-static --reset -p yes # This step will execute the registering scripts


go to the ros_bridge_arm_docker directory and run docker build --platform linux/arm64 -t tag_name -f Dockerfile_name  .

to run the docker go to the ros_bridge_arm_docker directory and run '''docker compose up'''
or ''' docker-compose up''' depending on the verision of docker compose that you have. There are certain fields in the docker-compose.yaml file.
