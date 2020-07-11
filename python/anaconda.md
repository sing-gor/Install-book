# 安装Anaconda
直接到(Anaconda的下载页)[https://www.anaconda.com/products/individual]选择对应的操作系统进行下载。  
不用理会python的版本是否是你需要的版本，因为我们可以通过虚拟环境进行切换。  
**注意是下载python3**.
## Mac
下载后直接一直下一步下一步安装。没遇到过安装失败，故此略过。  
## Windows
下载后直接一直下一步下一步安装。  
如果出现报错，请检查你的权限是否为管理员权限。  
如果出现其他问题，可以把错误信息和截图发送到`yusing-wong@outlook.com`。  
我到时候会再查找原因。  
注意： Window7用户的话，尽量去下载2018年到2019年之间的版本（很大概率会安装失败）。  

## Linux
下载完成后，文件通常都是在`/home/username/Download`里面。  
把终端切换到Download里面。  
输入`bash Ana`，然后按一下`tab`键，就可以自动补全命令了。  

如果是安装了**zsh**的话执行下面的做法。   
输入`zsh Ana`，然后按一下`tab`键，就可以自动补全命令了。  

命令会补全成  
`bash Anaconda3-5.2.0-Linux-x86_64.sh`  
或  
`zsh Anaconda3-5.2.0-Linux-x86_64.sh`  
这个会根据下载的版本号来决定的。   
运行代码后，根据提示按下回车，直到提示你输入**yes or no**,  
这里毫无意外肯定是输入**yes**
等待它安装，中途会询问你安装到那个文件夹，正常按下`回车`即可，安装到用户的根目录下。  
如果你有其他需求可以设定其他的目录下。  
继续等待安装，然后又出现一个对话框问你是否把Anaconda添加到环境变量中，选择**yes**  
最后，Anaconda安装完成后会询问你是否安装**VScode**，这个根据自身需求吧。我没有安装，输入**no**即可。  
### 检查是否安装成功  
关闭当前终端，新开一个终端。  
输入`python`  
可以看到python变成3.61了。  
当然未来的你可能会看到3.7或3.8甚至4.x。   

### python仍然是2.7的处理方法   
原因是因为，安装了**zsh**的情况下仍然执行`bash Anaconda3-5.2.0-Linux-x86_64.sh` 进行安装。  
导致Anaconda的环境变量未加入到zsh中。   
需要依次执行下方命令。（注意，需要把下面路径中的username替换成你的用户名）   
`echo 'export PATH="/home/username/anaconda3/bin:$PATH"' >> ~/.zshrc`    
重新加载配置文件  
`source ~/.zshrc`


## 测试是否安装成功  
在终端输入`conda -V`查看anaconda的版本号。  

如果显示**找不到该命令路径**。  
请把错误复制到搜索引擎中查找解决方案。  
例如：  
* mac anaconda 环境变量设置
* windows anaconda 环境变量设置
* linux anaconda 环境变量设置
