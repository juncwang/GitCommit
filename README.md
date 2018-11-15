
### Git 的安装方法

1. Mac
    * `http://git-scm.com/download/mac`

2. Windows
    * `http://git-scm.com/download/win`

3. 配置 Git 
    1. 打开终端运行 $ cd ~/.ssh
    2. 生成SSH KEY $ ssh-keygen -t rsa -C juncwang@live.com
    3. 连续按下回车键进行生成
    4. 打开终端运行 $ open ~/.ssh
    5. 查看 id_rsa.pub 的内容并进行复制
    6. 登陆 GitHub 进入个人设置内添加 SSH KEY


### Git 命令行命令

1. `git --version`                                  查看 Git 版本
2. `git config --global user.name 'UserName'`       配置使用者名称
3. `git config --global user.email 'UserEMail'`     配置使用者邮箱
4. `git status`                                     查看状态
5. `git add <file>`                                 添加文件
    * `git add *.html`                              添加所有 html 文件
    * `git add .`                                   添加所有文件
6. `git rm --cached <file>`                         删除添加的文件
7. `git commit`                                     提交备注所需添加文件的信息
    * `git commit -m 'Remarks'`                     提交备注所需添加文件的信息-简便方式, 不需要进入 vim
8. `.gitignore`                                     创建忽略文件对不想上传的文件在该文件内写入进行忽略
    * `fileName.txt`                                忽略文件
    * `/dir`                                        忽略文件夹
9. `git branch Name`                                创建一个分支
    * `master`                                      主线名称不可更改-分支不可同名
    * `Name`                                        分支名称-可以使用自己希望的名称
10. `git checkout Name`                             切换到分支
11. `git merge Name`                                在 master 下使用该命令把对应的分支代码合并到主线内
12. `git remote add origin httpAddres`              设置连接远程仓库
    * `git remote`                                  查看是否连接远程仓库
13. `git push -u origin master`                     推送到仓库
14. `git clone httpAddres`                          从远程仓库拷贝数据
15. `git pull origin`                               从远程仓库拉取数据