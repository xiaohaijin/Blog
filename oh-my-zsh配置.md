## oh-my-zsh安装和配置

oh-my-zsh是一个zsh命令行的一个扩展工具集，驱动的命令行工具，提供了主题配置、插件机制、已经内置的便捷操作，给我们一种全新的方式使用命令行，oh-my-zsh的官方网址是[ohmyz.sh](https://ohmyz.sh)

### 安装方法

首先切换到zsh作为命令行的sh
```bash
chsh 
```
选择自己的zsh。


采用wget的安装方法
```bash
wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | sh
```

安装语法高亮插件
```bash
cd ~/.oh-my-zsh/custom/plugins
git clone git://github.com/zsh-users/zsh-syntax-highlighting.git
```

修改.zshrc配置文件
```bash
ZSH_THEME="xiaohai"
HYPHEN_INSENSITIVE="true"
DISABLE_AUTO_UPDATE="true"
ENABLE_CORRECTION="true"
COMPLETION_WAITING_DOTS="true"
plugins=( git z zsh-syntax-highlighting)
```

至此.zsh的配置就算完成了
