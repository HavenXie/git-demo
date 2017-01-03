#### 5.3.1.初始化一个本地GIT仓储
```
// 定位到仓储文件夹目录
$ cd /dir
// 初始化本地仓储
$ git init
```

#### 5.3.2.添加本地GIT忽略清单文件.gitignore
```
// 添加OS X中系统文件.DS_Store到忽略清单，这将忽略项目任意目录下的.DS_Store文件或是文件夹
$ echo .DS_Store >> .gitignore
```

#### 5.3.3.查看本地仓储的变更状态
```
$ git status
```

#### 5.3.4.添加本地暂存（托管）文件
```
// 添加指定文件名的文件
$ git add README.md
// 添加通配符匹配的文件
$ git add *.md
// 添加所有未托管的文件（忽略.gitignore清单中的列表）
$ git add --all
```

#### 5.3.5.提交被托管的文件变化到本地仓储
```
$ git commit -m 'Initial commit(change log)'
```

#### 5.3.6.为仓储添加远端（服务器端）地址
```
// 添加一个远端地址并起了一个别名叫origin
$ git remote add origin https://github.com/HavenXie/git-demo.git
// 查看现有的远端列表
$ git remote -v
```

#### 5.3.7.将本地仓储的提交记录推送到远端的master分支
```
$ git push -u origin master
```

#### 5.3.8.拉取远端master分支的更新记录到本地
```
$ git pull origin master
```



