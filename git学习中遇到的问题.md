# 端口超时解决方案

#### 我们在GitHub上添加完SSH key之后，在Git上验证SSH key是否绑定成功是可能会遇到端口超时的问题，此时则可以输入vim ~/.ssh/config点击回车后会进入一个新界面

#### 在这个界面我们按格式输入

#### Host github.com

#### Hostname ssh.github.com

#### Port 443

#### 后再按住ESC输入 :wq即可（此处注意:也要输入）

#### 后续可能会有如下情况，这是在确认你是否相信改服务器，输入yes即可

![image-20251107200255808](C:\Users\LEGION\AppData\Roaming\Typora\typora-user-images\image-20251107200255808.png)

#### 之后再输入ssh -T git@github.com检查是否能正常链接

# SSL证书验证不通过问题

#### 在拉取（pull）和推送（push）可能会有SSL证书验证不通过的情况

#### 此时可以手动配置证书

#### 输入git config --global http.sslCAlnfo "D:\Git\mingw64\etc\ssl\cert.pem"

#### ""中的为证书在本地的路径，这个需要自己去找

#### 一般这样配置之之后就不会出现问题了

# Git拒绝合并问题

#### 比如在拉取远程仓库时，本地的文件比远程仓库的文件更新，就会出现这样的情况

#### ![image-20251109203311404](C:\Users\LEGION\AppData\Roaming\Typora\typora-user-images\image-20251109203311404.png)

#### 这是Git出于安全考虑拒绝合并，可以在git pull命令后加上`--allow-unrelated-histories`

#### `git pull origin master --allow-unrelated-histories`

