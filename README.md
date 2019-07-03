nginx-php-supervisor-composer-crond  容器直接build 并run运行即可。
特点如下：
1，以世界上最小的linux系统(alpine)为核心，仅5M的系统，最适合作为容器的操作系统。
2，该项目集成了 nginx 1.13，开箱即用。
3，该项目集成了 PHP7.2,并且nginx已连通php，只要在/var/share/nginx/html/public 目录下放入php项目即可访问。
4，该项目还集成了supervisor，可以监控进程，重启进程，使用场景比如，队列进程的监控 重启等。
5，项目集成了composer，PHP包管理工具。
6，该项目也集成了crond，即定时器。定时文件 默认在/etc/crond/下的root文件，该文件可以自己再重写进去，有一个laravel的示例定时执行任务，默认#注释了的，可以去掉#号自行开启与编写。

tips：本项目制作而成的镜像，主要用于PHP项目，php 的laravel项目没有任何问题。
镜像地址：https://hub.docker.com/r/liudashuai/docker-nginx-php-supervisor-simple
