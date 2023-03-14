### FROM
* Set a base image, Docker file must start with from instruction
```
 FROM <image>[:<tag>] [AS <name>]
```
Where 
* image : Name of the base image,
* tag: specifies a particular version of the image( Docker will use     the latest tag by default),
* AS <name>: Image name for future reference

### RUN
* The RUN instruction is used to install packages, update the system, download and install software, copy files, and perform any other necessary operations to configure the Docker image during the build process.
* each RUN instruction creates a new layer in the Docker image

### CMD
* The main purpose of a CMD is to provide defaults for an executing "container"
* it can also be overridden by passing a new command as an argument when starting the container
* Ways to represent CMD instruction:
 * CMD ["executable","param1","param2"] (exec form, this is the preferred form)
 * CMD ["param1","param2"] (as default parameters to ENTRYPOINT)
 * CMD command param1 param2 (shell form)
* Note: it's recommended to use the exec form instead of the shell form in Dockerfiles, since it's more secure and less error-prone
* There can only be one CMD instruction in a Dockerfile. If you list more than one CMD then only the last CMD will take effect
* CMD does not create a new layer in the Docker image

### Difference between RUN and CMD
* RUN is used to modify the image during the build process were as 
* CMD should be executed when a container is started from the image
