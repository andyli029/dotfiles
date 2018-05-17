# config for software

- vim
- ycm config
- zsh

## vim 
- install vim 8.0 
    - mac ` brew install vim --with-override-system-vi `   install [homebrew](brew.sh)
    - linux 
        1. `yum remove vim-* -y`
        2. `wget -P /etc/yum.repos.d/ https://copr.fedorainfracloud.org/coprs/mcepl/vim8/repo/epel-7/mcepl-vim8-epel-7.repo`
        3. `yum -y install vim-enhanced sudo`
- clone dotfiles
    - ` git clone https://github.com/jzdxeb/dotfiles.git [-b mac ]` -b 参数可选

- create link 
    - ` ln -s $(DOTFILEPATH)/config/vimrc $(HOME)/.vimrc`
    - ` ln -s $(DOTFILEPATH)/vim $(HOME)/.vim`
- install vim plugin
    - `  vim +PlugInstall +qall `
*PS*: vim-go 插件安装需要翻墙配置代理
# [http]
#     proxy = socks5://127.0.0.1:8899
#[https]
#     proxy = socks5://127.0.0.1:8899

#cp $(DOTFILEPATH)/vim/.ycm_extra_conf.py /root/.ycm_extra_conf.py


## zsh 
- 修改默认shell
    - linux `chsh -l`查看是否存在zsh 存在使用 `chsh -s /bin/zsh` 不存在 `yum install zsh`
    - mac `chsh -l`查看是否存在zsh 存在使用 `chsh -s /bin/zsh`不存在 `brew install zsh`
- clone dotfiles 同上
- clone oh-my-zsh
    - `git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh`
- create link 
    - ` ln -s $(DOTFILEPATH)/config/zshrc $(HOME)/.zshrc`
- restart terminal


## vim plugin
TODO
## zsh plugin
TODO
