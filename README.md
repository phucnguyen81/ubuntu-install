# ubuntu-install 项目简介
在使用ubuntu时，我们总会有各式各样自己的配置，比如安装自己习惯的编辑器，自己喜爱的终端软件，功能更好的截屏软件，以及各式各样的配置。
这个配置是很个性化，是不断积累的。可是呢，我们在公司，在同事电脑，或者各种其他情况，使用不是自己电脑的时候，又想使用自己的环境配置时，重新配置就会非常麻烦。
因此我的做法时，将自己所有软件安装或者环境配置，都写成脚本。然后通过存放在该项目中。这样无论在什么电脑上，当我需要某个环境时，都很很快的部署安装。而不必重新开始。并且也做了备份。不用担心电脑故障而丢失。

## 下载到本地
```
cd ~
git clone https://coding.net/qinshulei/ubuntu-install.git
cd ubuntu-install
git submodule init
git submodule update
```

## 全部安装
```install
cd ~/ubuntu-install
./install
```

## 局部安装

### [guake](https://github.com/Guake/guake/) 安装 ： 一款很好用的终端
```install
cd ~/ubuntu-install
./software-install/install-guake
```

### [shutter](http://shutter-project.org/) 安装 : 截屏软件
```install
cd ~/ubuntu-install
./software-install/install-shutter
```

### [emacs](http://www.gnu.org/software/emacs/) 安装 ： 功能最强大的文本编辑器，没有之一
```install
cd ~/ubuntu-install
./software-install/install-emacs24
./settings/emacs-setting/init-with-purcell-setting
```

### [node](http://www.nodejs.org/) 安装 ： nodejs 环境
```install
cd ~/ubuntu-install
./software-install/install-nodejs
./npm-install/install-yo-bower-grunt
```

### [ruby](https://www.ruby-lang.org/en/) and [compass](http://compass-style.org/) 安装 ： 如果使用 grunt 之类的自动化工具会依赖它
```install
cd ~/ubuntu-install
./software-install/install-ruby-and-compass
```

### [mongodb](http://www.mongodb.org/) 安装 ： nosql数据库
```install
cd ~/ubuntu-install
./software-install/install-mongodb
```

### [zsh](http://www.zsh.org/) and [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh/) install ： 交互性更好install，兼容bash，但有着更优秀的补全。使用oh-my-zsh作为配置
```install
cd ~/ubuntu-install
./software-install/install-zsh
```

### [ack](http://beyondgrep.com/) install : grep 的一个替代品，内置多种代码文件类型，非常适合源码搜索。
```install
cd ~/ubuntu-install
./software-install/install-ack
```

### [htop](http://hisham.hm/htop/) : top 的替代品 ，交互更好
```install
cd ~/ubuntu-install
./software-install/install-htop
```
