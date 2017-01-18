# myTest
mytest

#生成SSH公钥

git config --global user.name "yourName" #配置用户名
git config --global user.email "yourEmail" #配置邮箱
ssh-keygen -t rsa -C "yourEmail" #生成SSH公钥
cat ~/.ssh/id_rsa.pub #查看公钥，并把次公钥添加到[个人设置-SSH keys]
ssh -T git@github.com #若返回You've successfully authenticated, but GitHub does not provide shell access 。这就表示已成功连上github。 

#config

git config --list #查看当前git配置