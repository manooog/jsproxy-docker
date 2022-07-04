## 自编译过程

https://github.com/EtherDream/jsproxy/blob/master/docs/setup.md

## 直接走测试

docker run --rm -it $(docker build -q .) sh


## 编译多平台

docker buildx build --platform linux/amd64,linux/arm/v8 .