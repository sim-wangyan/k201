# Gitlab部署和基本使用

## 安装Docker

参考Harbor安装文档进行Docker安装。

## 启动Gitlab

    $ docker run --detach \
        --hostname git.hipstershop.cn \
        --publish 6443:443 --publish 8000:80 --publish 2222:22 \
        --name gitlab \
        --restart always \
        --volume /data/gitlab/config:/etc/gitlab \
        --volume /data/gitlab/logs:/var/log/gitlab \
        --volume /data/gitlab/data:/var/opt/gitlab \
        gitlab/gitlab-ce:latest
