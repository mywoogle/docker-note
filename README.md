# sourcetree_gitflow_Multi-Version-Concurrency
git Multi-Version Concurrency release,use gitflow,on surcetree.source tree gitflow  Multi-Version Concurrency release

# Description
The script will change the current master/develop of sourcetree,according to current branch.

# How To Use
1.  copy the sourcetree_gitflow_Multi-Version-Concurrency.sh to any folder,example C:\Users\woogle\Desktop\sourcetree_gitflow_Multi-Version-Concurrency.sh
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/1.png)
2.  cd /path/to/repository   and run "bash /C/Users/woogle/Desktop/sourcetree_gitflow_Multi-Version-Concurrency.sh"
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/101.png)
###OR use sourcetree's custom aciton###
####Create dourcetree's custom action####
![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/201.png)
####Run sourcetree's custom action####
######action>>custom action>>Multi-Version Concurrency######
![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/202.png)

3.  add Multiple versions of master in sourcetree,the format as master_version
    example,master_qq,master_sina
        ![image](https://github.com/mywoogle/sourcetree_gitflow_Multi-Version-Concurrency-release/blob/master/image/2.png)
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
