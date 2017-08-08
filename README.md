# [ffmpeg-and-node Docker Image](https://hub.docker.com/r/karuppiah7890/ffmpeg-and-node/)
I wanted node and ffmpeg in a very small Docker container for one of my projects. The plan was to get a mix of node:alpine and jrottenberg/ffmpeg:3.3-alpine, both of which are based on alpine os Docker images. So I used the base image as jrottenberg/ffmpeg:3.3-alpine and used the instructions in node:alpine to build nodejs v8.2.1 from source and to get yarn v0.27.5 binaries too. 

Run the below command in the terminal to work with a shell which has ffmpeg, nodejs and yarn installed

```
docker run --name ffmpeg-node -i -t karuppiah7890/ffmpeg-and-node:latest
```