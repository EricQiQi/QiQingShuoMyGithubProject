创建基于GitHub的毕设项目
1.安装git

1.1下载git

1.2安装git


2.注册github帐户

3.创建GitHub仓库（repository）
仓库名字以“姓名项目名”方式命名，使用驼峰拼写

4.创建公钥私钥
4.1配置git帐户
...
配置的git帐户
git config --global user.name "QiQingShuo"
git config --global user.email "********@qq.com"
...
生成的文件在
C:\Users\26819\.ssh

4.2创建密钥

4.3将公钥‘id_rsa.pub'中的内容在GitHub中建立密钥
GitHub settings----SSH and GPG keys----SSH keys->new SSH key

5.将GitHub上建立的项目clone到本地，如e盘下某个目录
打开git.cmd
   C:...  -->E:
   E:/   -->cd ...
   E:...  -->git clone (项目ssh私钥)
                    yes
   
6.修改后同步文件
用 'syn.bat'

7.idea中进行git操作
项目文件夹-->git-->commit directory将要上传的文件选中，然后push
如果第一次使用idea上传，会遇到push被拒绝，见如下链接解决问题
https://blog.csdn.net/qq_36522306/article/details/94390588
不是使用idea操作的文件，仍然使用'syn.bat'同步

