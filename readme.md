# jsprxy-docker

该项目是为 jsproxy 构建 docker 镜像而创立的，全程参考了[jsproxy 自编译过程](https://github.com/EtherDream/jsproxy/blob/master/docs/setup.md)，可放心使用。

目前，镜像支持 x86 和 arm64。

## 直接走测试

docker run --rm -it $(docker build -q .) sh


## 编译多平台

docker buildx build --platform linux/amd64,linux/arm/v8 .