##  Git 操作


#### 基本操作

- 查看当前git状态  
git status 

- 添加代码到暂缓区  
git add .

- 提交代码到本地  
git commit -m ''

- remote 远程仓库  
git remote add origin https://远程仓库

- push 到远程仓库  
git push origin master

- 版本标签  
  git tag   
  git tag '版本'  
  git push --tags
- 删除tag
  - 删除本地tag   
    git tag -d 版本号  
  - 删除远程tag  
    git push origin --delete tag 版本号


## Cocoapods

### 基本操作
- 创建spec文件   
 pod spec create 名字

- spec文件描述
  - s.name  项目名字
  - s.version 项目版本
  - s.summary 项目摘要
  - s.homepage 项目网站（github 上的网址）
  - s.license 项目协议
  - s.author 项目作者
  - s.source 项目映射地址
  - s.source_files 指定下载文件

- 提交审核  
  pod trunk register 邮箱 '名字' --verbose  
  pod trunk push spec文件.podspec
  
- 验证审核  
  pod spec lint   spec文件.podspec
- 私有库pod  
  pod '库的名字', :path => '路径'
  