### 配置多个仓库

在开发中，我们将公司的代码提交到公司自己的远程仓库。但是我们平常自己的项目可能会传到Coding或者Github上，这个时候就需要我们一台电脑有能力提交到不同的远程仓库



### 创建密钥

我的电脑已经生成了Coding的密钥，我再生成一个github的密钥，

> 注意：这个不能一直按回车了，要不把Coding的密钥覆盖掉了

![](https://tva1.sinaimg.cn/large/006tNbRwgy1gap8ti78m6j31yo0mcwm0.jpg)

查看.ssh文件夹

![](https://tva1.sinaimg.cn/large/006tNbRwgy1gap8urjoxgj31yk094q4q.jpg)

这样就生成了两对密钥。

### 配置Github公钥

![](https://tva1.sinaimg.cn/large/006tNbRwgy1gap8y9xrkyj31yw0cwwht.jpg)

### 配置文件

在.ssh文件下创建一个名字为config的文件

![](https://tva1.sinaimg.cn/large/006tNbRwgy1gap8w188xij31wq05yq3z.jpg)

文件内容如下

```
Host github
HostName github.com
User git
IdentityFile ~/.ssh/id_rsa_github


Host coding
HostName coding.net
User git
IdentityFile ~/.ssh/id_rsa
```



### 问题解决

![](https://tva1.sinaimg.cn/large/006tNbRwgy1gap8ylixzuj31ys0gijxf.jpg)

```
ssh-add ~/.ssh/id_rsa_github
```

![](https://tva1.sinaimg.cn/large/006tNbRwgy1gap8zf51ocj31qk06kq55.jpg)