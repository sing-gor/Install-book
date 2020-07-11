# Install Ruby
由于windows上安装和使用ruby的过程比较难。  
且不推荐在Window上开发和运行ruby。  
故此，只介绍Mac和Linux上的安装


## Mac和Linux安装Ruby  
安装ruby最好是使用RVM进行安装。  
先到[rvm的官网](https://rvm.io/)依次复制并执行前两条命令。  
稍待片刻，即可完成rvm的安装。   

安装完成后，选择稳定的版本进行安装  
`rvm list known`  
目前选择是2.5.1  
`rvm install 2.5.1`  
安装完成后，输入`ruby -v`  
如果出现错误。说明没有配置环境变量。   
终端下的依次输入下面的语句即可成功。（注意，需要把下面路径中的username替换成你的用户名，注意如果你没有使用zsh，请替换为你使用的终端机，例如bash）    
`echo 'export PATH="/home/username/.rvm/rubies/ruby-2.5.1/bin:$PATH"' >> ~/.zshrc`  
加载配置文件   
`source ~/.zshrc`  
