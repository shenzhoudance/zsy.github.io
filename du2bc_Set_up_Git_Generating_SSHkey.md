
# [LOG]Set up Git n Generating SSH key
本文所有操作命令

`git --version`

`git config --global user.name "zhangshiyinrunwithcc"`

`git config --global user.email "981318360@qq.com"`

`ls -al ~/.ssh`

`cd ~/.ssh`

`mkdir key_backup` 

`cp id_rsa* key_backup`

`cat ~/.ssh/id_rsa.pub`

`ssh-keygen -t rsa -C "example@qq.com"`

`ssh -T git@github.com`

本文阅读配置说明

### 标题 (期待实现的功能)

Link > (参考资料)

CML > (操作命令行)

Return > (终端反馈)
```
(终端反馈)
```

Further Reading > （相关文档）

### 检查Git版本
Link > [Git version](https://help.github.com/articles/set-up-git/)

CML > `git --version`

Return > 
```
git version 2.10.1
```


### Set up Git

Link > [Set up Git](https://help.github.com/articles/set-up-git/)

CML > `$ git config --global user.name "zhangshiyinrunwithcc"` `$ git config --global user.email "981318360@qq.com"`

Return > 
```

```

### 检查是否已有public ssh key

Link > [Connecting to GitHub with SSH - User Documentation](https://help.github.com/articles/connecting-to-github-with-ssh/)

CML > `ls -al ~/.ssh`

Return > 
```
total 24
drwx------   5 zhangshiying  staff   170 Dec  3 10:31 .
drwxr-xr-x+ 48 zhangshiying  staff  1632 Mar 29 14:47 ..
-rw-------   1 zhangshiying  staff  1766 Dec  3 10:49 id_rsa
-rw-r--r--   1 zhangshiying  staff   398 Dec  3 10:49 id_rsa.pub
-rw-r--r--   1 zhangshiying  staff   803 Dec  3 10:42 known_hosts
```

### 暂时不用原来的sshkey

Goal > 暂时不用原来生成的ssh key, 就把它们存到其他目录下

CML > `mkdir key_backup` `cp id_rsa* key_backup`

### 生成新的ssh key
Goal > 生成新的ssh key, 并绑定邮箱

CML > `ssh-keygen -t rsa -C "981318360@qq.com"`

Return > 终端返回, 新的rsa key pair已经生成, 然后一路回车, 输入passphrase
```
Generating public/private rsa key pair.
Enter file in which to save the key (/Users/zhangshiying/.ssh/id_rsa):
/Users/zhangshiying/.ssh/id_rsa already exists.
Overwrite (y/n)? yes
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
```

Return > 新的public key已经被保存在id_rsa.pub里
```
Your identification has been saved in /Users/zhangshiying/.ssh/id_rsa.
Your public key has been saved in /Users/zhangshiying/.ssh/id_rsa.pub.
```

### 打开/复制public ssh key文件

Link > [how-do-i-access-my-ssh-public-key](http://stackoverflow.com/questions/3828164/how-do-i-access-my-ssh-public-key)

CML > `cat ~/.ssh/id_rsa.pub`

Return > 
```
zhangshingdeAir:.ssh zhangshiying$ cat ~/.ssh/id_rsa.pub
ssh-rsa AAAAB3Nza...981318360@qq.com
```

### 将public ssh key粘贴到github setting中

Link > 

CML > 复制粘贴

Further Reading > [Generating a new SSH key](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/)

### 测试SSH与Github的连接

Link > [Testing your SSH connection](https://help.github.com/articles/testing-your-ssh-connection/)

Goal > 测试连接

CML > `ssh -T git@github.com`

Return > 终端返回`Hi zhangshiyinrunwithcc! You've successfully authenticated, but GitHub does not provide shell access.`, 连接成功！
