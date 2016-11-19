# blog.github.com
上传时的准备工作：
	1.本地生成一个秘钥
		在cmd 中输入
		ssh-keygen  -C "18500995124@163.com" -t rsa
		然后一路回车，默认就行->window系统去，当前C盘，当前用户列表里面找到.ssh文件夹，里面有两个文件：
		id_rsa  私有秘钥（千万不能给别人）只能用记事本打开
		id_rsa.pub 共有秘钥  
	2.把秘钥放到github
		头像->settings->SSH and GPG keys->new SSH Key
	3.配置一下我是谁
		git config -–global user.name 'name'		
		git config -–global user.email '必须是你的注册邮箱'
	本地代码扔到github上：
		第一次：
			跟github建立关系
				git remote add origin 	'文件链接地址'
			推送到 github
			git push -u origin master
		以后：	
			git add->git commit->git push
