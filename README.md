# 进度
- 14.04环境JDK7和JDK8均已配置完毕，待测试编译环境效果
- 16.04环境JDK8和编译工具链理论上配置完毕
- 编译sh脚本未配置

# Docker镜像编译命令
docker build -f ./Dockerfile_14_04 -t aosp-build:14.04 .

docker run -itd --name aosp_builder aosp-build:14.04

docker exec -it aosp_builder /bin/bash

# 致谢
- https://github.com/Tinker-S/docker-android-build
- https://github.com/Lagranmoon/aosp-build-env/blob/master/Dockerfile