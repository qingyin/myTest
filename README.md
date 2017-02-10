# myTest
mytest

#生成SSH公钥
git config --global user.name "yourName" #配置用户名

git config --global user.email "yourEmail" #配置邮箱

ssh-keygen -t rsa -C "yourEmail" #生成SSH公钥

cat ~/.ssh/id_rsa.pub #查看公钥，并把次公钥添加到[个人设置-SSH keys]https://github.com/settings/keys

ssh -T git@github.com #若返回You've successfully authenticated, but GitHub does not provide shell access 。这就表示已成功连上github。 

#config
git config --list #查看当前git配置

#add
git add demo.txt #添加指定文件到暂存区

git commit demo.txt -m "add file demo.txt" #提交暂存区到仓库区(本地仓库区)

git commit -v #提交时显示所有diff信息

git push #上传本地仓库到远程仓库

#add locate project to remote git
git init

git add .

git commit -m "add current folder[children folder]"

git remote add origin git@github.com:qingyin/XX.git

git push -u origin master
