#关于python的一些知识点


## pythonbrew 
==========================
安装
首先你得装一个 python 吧，这里只在 Unix-like 系统下进行， Windows 上没有试过。你有两种简单的安装方法，easy_install:

[sudo] easy_install pythonbrew
或者 pip：

[sudo] pip install pythonbrew
即可安装完成。

然后在你的 ~/.bashrc 或者 ~/.zshrc 文件中追加下面这一行，重启终端即可：

[[ -s $HOME/.pythonbrew/etc/bashrc ]] && source $HOME/.pythonbrew/etc/bashrc
使用
列出可安装的 python 版本：pythonbrew list --know

安装某个版本的 python ： pythonbrew install 2.7.3

删除已安装的某版本的 python ： pythonbrew uninstall 2.7.3

列出已安装的 python 版本(当前使用的版本后会用星号标记)： pythonbrew list

使用某个版本的 python （仅当前终端窗口有效)： pythonbrew use 2.7.3

切换到某个版本的 python （一直有效）： pythonbrew switch 2.7.3

清理陈旧的源码目录和档案包： pythonbrew cleanup

升级到pythonbrew到最新版本： pythonbrew update

禁用pythonbrew(即切换回原始环境)： pythonbrew off

创建python隔离环境(借助virtualenv)：

pythonbrew venv init

pythonbrew venv create proj

pythonbrew venv list

pythonbrew venv use proj

pythonbrew venv delete proj

pythonbrew venv rename proj proj2
查看 pythonbrew 版本： pythonbrew version
