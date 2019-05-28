DevOps 演示项目

1.使用Git Bash生成证书

  $ssh-keygen.exe -t rsa

2.切换到用户家目录的.ssh目录下

  $cd ~/.ssh

3.列出目录下所有文件

  $ ls
  id_rsa  id_rsa.pub
  
4.查看文件内容

  
  $ cat id_rsa.pub
  
2.把公钥id_rsa.pub的内容放置到github上。

打开Github。点击用户图像--Settings--SSH and GPG keys--New SSH

3.克隆仓库代码

  git clone git@github.com:su-cloud/devops.git
  
4.编写代码

  cd ~/Desktop/devops
  
  git status
  
  git add README.md
  
  git commit -m "第一次提交" README.md
  
  git push


5.提交时如果不成功，出现提示，就需要设置你的邮箱和用户名

  git config --global user.email "you@example.com"
  
  git config --global user.name "Your Name"
  
把邮箱替换为你的,用户名替换为你的用户名.
