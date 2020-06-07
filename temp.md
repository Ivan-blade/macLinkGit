### 安装步骤
+ 安装xcode
+ 查看git版本
  + git --version
+ 生成ssh key
  + ssh-keygen -t rsa -b 4096 -C "email"
+ 一直回车直到密钥生成完毕
+ 提取rsa
  + cat /Users/root/.ssh/id_rsa.pub（默认是这个，以上一步系统生成密钥后提示的为主）
+ 将查询到的密钥复制粘贴到github - setting - ssh and gpg keys中的ssh中，标题随意
+ 在本地配置github用户名和邮箱
  ```
	git config --global user.name "用户名"
	git config --global user.email "邮箱"
  ```
+ 测试链接
  + ssh -T git@github.com（可能需要回车一下）
