## 下载git

```cpp
https://git-scm.com/downloads
```



## 配置用户名和邮箱

```csharp
git config --global user.name "your_name"  
git config --global user.email "your_email@youremail.com"
```



## 查看git的配置信息

```
git config --list
```



## 设置为大小写敏感

```bash
git config core.ignorecase false
```



## 生成密钥

```css
ssh-keygen -t rsa -C "your_email@youremail.com"
```

- 本地的/Users/当前电脑用户/.ssh目录下会生成两个文件id_rsa、id_rsa.pub，id_rsa文件保存的是私钥，保存于本地，id_rsa.pub文件保存的是公钥，需要将里面内容上传到远端仓库。



## sGitHub 添加new ssh key

1. 打开你的github账号，在`Settings`中的左侧边导航中找到`SSH and GPG keys`，点击左面面板右上方的`New SSH key`添加密匙。
2. `Title`填写自己的备注标题名称（自定义），`Key`填写刚才`id_rsa.pub`中的内容.



## 将项目clone 到本地

```
git clone url
```



## 拉取更新到本地

将远程主机 origin 的 master 分支拉取过来，与本地的 brantest 分支合并。

```
git pull origin master
```



## 提交代码

- 提交到缓存

```
git add .     #把新增的、修改的都加到缓存
```

```
git add -A    #把新增、和修改的、和删除的都加到缓存
```

- 从缓存中加到本地库

```
git commit -m “描述”
```

- 推送到远程库

```
git push origin master
```



## 删除本地指定的远程地址

```
git remote remove origin
```



## 添加远程地址

这里使用ssh链接才行

```
git remote add origin https:``//xxxxxxxxxxxx.git
```

