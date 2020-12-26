## git只显示提交时间和说明
> git log --graph --pretty=format:"%C(yellow)%h%x09%Creset%C(cyan)%C(bold)%ad%Creset  %C(green)%Creset %s" --date=format:'%Y-%m-%d %H:%M:%S'

## git 遇到 “could not read Username for 'http://git.code.oa.com': No such device or address”

> git pull , 输入账号密码
> git config --global credential.helper store
