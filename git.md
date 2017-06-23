## git的安装
* 在命令行下执行sudo apt-get install git
* 将software.git下载下来，执行git clone https://github.com/wanglei/software.git
* ls看当前目录下是否已存在，再进入目录cd sofeware/
* ls –a看当前目录下存在的文件，包含隐藏文件，找到install.sh，运行./install.sh
## 创建版本库及使用

1. 先要创建一个目录, 这个目录就是用来存放仓库的：mkdir github，然后进入目录cd github

2. 使用git init命令, 将当前目录创建成git仓库：git init

3. la -a会发现有一个隐藏的.git目录

4. 增加文件touch README或者vim README

5. 查看文件状态：git status，此时查看到的文件是红色的

6. 把文件加到仓库中去, 只有加到仓库中了, 才可能看到文件的变化: 

7. git add README，此时再git status，则文件变为绿色

8. 配置用户名：git config --global user.name

9. 配置用户邮箱：git config --global user.email

10. 配置编辑器：git config --global core.editor vim

11. 提交：git commit

12. 查看提交信息：git log

13. 比较前后两次提交的变化：git diff

