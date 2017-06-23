
## ubuntu安装

1. 在VMware中点击create a new virtual machine。
2. 进入安装界面后，点击next，之后选择已下载的Ubuntu镜像的路径。
3. 继续点击next，如所示，设置自己的用户名linux和密码1。
4. 继续点击next，在location中，选择自己的安装路径。
5. 继续点击next，在maximum disk zjze 中，把空间设置大一点。
6. 点击next，直到finish。


## Linux环境下文件基本操作

1. 新建文件：touch  file
2. 将file复制到file1：cp file file1
3. 将file复制到另外一个目录下的file1：cp file  /home/linux/file1
4. 重命名：mv file file2
5. 把file移动到另外一个目录中：mv file  /home/linux/
6. 查看文件权限及类型等：ls -al 
7. 查看文件内容：cat file

## Linux环境下目录基本操作

1. 新建一个目录：mkdir dir
2. 拷贝目录：cp dir   dir1  -a
3. 拷贝目录：cp dir   /home/linux/dir2  -a
4. mv dir  dir2
5. mv dir  /home/linux/
6. 删除：rm  dir  -rf
7. find  ./dir  -name  "filename"

## 文件的归档和压缩
* tar:      打包压缩
* -c        归档文件
* -x        压缩文件
* -z        gzip压缩文件
* -j        bzip2压缩文件
* -v        显示压缩或解压缩过程 v(view)
* -f        使用档名
** tar -cvf /home/abc.tar /home/abc 只打包，不压缩 

## 系统管理命令
* stat      显示指定文件的详细信息，比ls更详细
* who       显示在线登陆用户
* whoami    显示当前操作用户
* hostname  显示主机名
* uname     显示系统信息
* top       动态显示当前耗费资源最多进程信息
* ps        显示瞬间进程状态 ps -aux
* du        查看目录大小 du -h /home带有单位显示目录信息
* df        查看磁盘大小 df -h 带有单位显示磁盘信息
* ifconfig  查看网络情况
* ping      测试网络连通
* man       命令不会用了 如：man ls
* clear     清屏
* kill      杀死进程，可以先用ps 或 top命令查看进程的id,然后再用kill命令杀死进程

