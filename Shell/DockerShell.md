## 启动docker
将宿主机的root目录挂在为容器的data0目录
> docker run -itd -v /root:/data0 --privileged --network host --name taftrpc 5018ff7445c7 /bin/bash
