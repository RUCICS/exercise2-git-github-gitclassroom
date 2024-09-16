# exercise2-git-github-gitclassroom
## 课前准备
在习题课完成之前，请完成以下配置
- Git在本机上的[安装](https://git-scm.com/downloads)
- 注册GitHub账号(如果你并没有注册的话),进入[GitHub](https://github.com/)注册即可，如有问题可参阅[官方教程](https://docs.github.com/zh/get-started/start-your-journey/creating-an-account-on-github)
- 完成Git在本机上的身份配置，也即
  ```shell
  git config --global user.name "Your name"
  git config --global user.email "YOUR_EMAIL"(使用注册的邮箱)
  ```
  如果你想要使用其它邮箱，还需要在GitHub中[配置提交邮件地址](https://docs.github.com/zh/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/setting-your-commit-email-address)
- 完成SSH配置    
  - 首先检测有没有密钥
  ```shell
  cd ~/.ssh
  ls
  //看是否存在 id_rsa 和 id_rsa.pub文件，如果存在，说明已经有SSH Key
  ```
  - 如果没有密钥，使用如下命令生成即可
  ```shell
  ssh-keygen -t rsa -C "xxx@xxx.com"
  //执行后一直回车即可
  ```
  - 将生成的id_rsa.pub中的内容复制到GitHub账户中即可
    `右上角`->`settings`->`SSH and GPG keys`->`New SSH`
- (如果你是Windows用户)完成Git在WSL中的安装与配置，如果感兴趣的同学可以参阅[教程中Git凭据管理器部分](https://learn.microsoft.com/zh-cn/windows/wsl/tutorials/wsl-git#git-credential-manager-setup)进行配置的共享。
