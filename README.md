# docker使用笔记
把在windows上使用docker踩的坑，记下了，备忘。

# Description
这里是一个备忘也是一个提升的过程记录

# How To Use
1.  安装dockertool

    1.1. 下载dockertool 官方地址是http://get.daocloud.io/#install-toolbox ，在https://get.daocloud.io/toolbox/ 这里下载国内镜像
    
    1.2. 安装请参考官方手册https://docs.docker.com/toolbox/toolbox_install_windows/
    
    1.3. 替换国内镜像源，具体方法参考http://docs.daocloud.io/faq/what-is-daocloud-accelerator#docker-toolbox

    1.4. 安装好后，点击桌面上的Docker Quickstart Terminal这快捷方式，会自动创建名字为default的dockervm，并启动。你会发现在这个启动的窗口中不能复制，很不方便，你可以安装最新版的git bash替换现在已经安装的，体验要好的多。在git-bash中输入docker-machine ssh，就可以进入刚刚启动的docker-vm。docker-machine start/stop分别为启动和关闭docker-vm，更多操作，请用docker-machine --help查看
    
2.  配置docker-vm

    2.0 执行docker-machine stop关闭docker-vm然后进行配置

    2.1 配置docker-vm与windows主机的共享目录：
    
    docker-vm创建时默认设置了一个共享目录c:/Users的映射，这个在docker-vm中应该有特殊的处理，可以在虚拟机里面看到，且是实时更新的，具体是如何处理的，现在还不太清楚。为简单我们就直接修改一下这个映射，是它映射到我们自己的目录就好了。如图![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/2.png)
    
    2.2 配置docker-vm网卡
    
    docker-vm默认添加了2个网卡，我们只需在“网卡1”中添加一条 127.0.0.1 80:80的转发就可以了。就这样修改后，就可以保证docker-vm既可以访问外网，也可以在windows上通过127.0.0.1，在浏览器上访问docker-vm的127.0.0.1。如图![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/2.png)
    
3.  add Multiple versions of master in sourcetree,the format as master_version
    example,master_qq,master_sina
        
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/3.png)
    
4.  add Multiple versions of develop in sourcetree,the format as develop_version
    example,develop_qq,develop_sina
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/4.png)
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/5.png)
    
5.  add a featue base on curent develop,format:_version_fearurename,example:_qq_feature1
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/6.png)
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/7.png)

6.  add a hotfix base on curent master,format:_version_hotfix1,example:_qq_hotfix1
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/8.png)
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/9.png)


# How To Use(OR use git hook)
1.  copy the post-checkout to /path/to/repository/.git/hooks,example D:\woogle_new\data\gittest\.git\hooks\post-checkout
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/301.png)

2.  add Multiple versions of master in sourcetree,the format as master_version
    example,master_qq,master_sina
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/2.png)
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/3.png)
    
3.  add Multiple versions of develop in sourcetree,the format as develop_version
    example,develop_qq,develop_sina
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/4.png)
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/5.png)
    
4.  add a featue base on curent develop,format:_version_fearurename,example:_qq_feature1
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/6.png)
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/7.png)

5.  add a hotfix base on curent master,format:_version_hotfix1,example:_qq_hotfix1
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/8.png)
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/9.png)

# License
Feel free to use it.
