## Docker

Docker是一个虚拟环境容器，可以将你的开发环境、代码、配置文件等一并打包到这个容器中，并发布和应用到任意平台中。

### 为什么要使用Docker?

#### 降低部署成本, 更加快速交付
对开发来说, 部署本地环境不再是一件头疼的事情.

比如安装最常见的LAMP环境, 不单单对基本组件的安装, 还需要对php安装拓展, 需要安装拓展需要的gcc,g++,openssl, 以及配置apache和mysql

安装完毕, 还需要自行检测组件安装是否工作, 中间耗费的时间成本和人力成本高, 并且可能安装系统崩溃, 无法运作, 浪费人力和时间.

更可怕的是, 在线上进行服务器迁移时, 对操作就更加严格了.

而, Docker使用镜像来构建容器, 以容器来打包应用, 从而得到标准的开发环境, 测试环境, 和线上环境, 大大降低了部署成本.

对于开发人员, 测试人员, 减少了在环境上浪费的时间, 实现产品的快速迭代和交付.

#### 轻量, 资源占用少
Docker是对内核级的虚拟化, 对资源的需求很低, 相比虚拟机, Docker在单机下可支持上千个容器运行.

#### 更简单的更新管理
使用Dockerfile, 只需要进行简单的配置修改, 即可替代以往大量的更新工作.

### Docker三大核心概念
- 镜像 (Image)
- 容器 (Container)
- 仓库 (Repository)