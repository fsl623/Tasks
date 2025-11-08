# git学习笔记

### 集中式与分布式的区别

- #### 集中式统的版本库是集中存放在中央服务器的，而干活的时候，用的都是自己的电脑，所以要先从中央服务器取得最新的版本，然后开始干活，干完活了，再把自己的活推送给中央服务器。中央服务器就好比是一个图书馆，你要改一本书，必须先从图书馆借出来，然后回到家自己改，改完了，再放回图书馆

  #### 且必须要联网才能工作，遇到网速慢得时候等文件就会花费很多时间

- #### 而分布式每个人的电脑上都是一个完整的版本库，这样，你工作的时候，就不需要联网了，因为版本库就在你自己的电脑上

# 注意

- #### 进行任何git操作前，必须先找到Git的仓库目录，即我们得到<u>先进入到（我们定义的）Git 仓库的最顶层文件目录下</u>，然后从此目录中进入 Git Bash

- #### 如选择demo目录作为 Git 仓库，然后进入demo目录之中，点击鼠标右键，再选择Git Bash Here，即可打开 Git Bash 的命令行窗口

<img width="450" height="422" alt="屏幕截图 2025-11-05 213536" src="https://github.com/user-attachments/assets/94d6b82f-b239-47ee-bc9b-4c3aef7d6dc6" />



- #### 在添加文件经git仓库时，所添加的文件一定不能是空文件，不然会导致系统找不到文件路径，或者直接添加文档而且文档也不能是空的

- #### 如图添加的readme.txt文档里一定要有东西
- <img width="1623" height="285" alt="屏幕截图 2025-11-07 184037" src="https://github.com/user-attachments/assets/b4adfaa6-573d-4650-a509-ddf308ef527a" />


# 一，命令语句

1. 1. #### git status：输入这个命令可以查看仓库状态，但此时显示demo不是git的仓库，还需在计算机中声明demo为git仓库
   2. <img width="759" height="143" alt="屏幕截图 2025-11-05 214046" src="https://github.com/user-attachments/assets/aaa9c485-ed3a-4efe-9d7a-038f482933d7" />

   3. #### git init：输入此命令，初始化Git仓库，此时已经将demo初始化为Git的仓库
   4. <img width="760" height="239" alt="屏幕截图 2025-11-05 214357" src="https://github.com/user-attachments/assets/f68bd8be-ee12-4c0b-a493-628341f5b46b" />


   5. #### git add：此命令是将文件放到缓存区，等待下一步给次文件的添加做说明

   6. #### git commit -m "text commit"：将缓存区文件提交到仓库，“ ”里的内容是对提交文件的标注，建议将文件提交的目的写清楚便于后续查看

   7. #### git log：打印Git仓库<u>提交</u>日志，会显示了我们的提交记录，提交记录的内容包括Author提交作者、Date提交日期和提交信息

   8. #### git branch：只输入git branch是查看Git仓库的分支情况；输入git branch a会创建一个名为a的分支，且当前仍处于主分支

   9. #### git checkout：输入git checkout a切换到a分支![img](https://pic1.zhimg.com/v2-3b28d0015bd823222db84211c034741e_1440w.jpg)

      #### 输入git branch -b b会直接创建一个名为b的分支并直接切换到b分支

      #### ![img](https://picx.zhimg.com/v2-bd7b115a3f411746658bf44eb78b00f9_1440w.jpg)

      #### 同时也该注意如果在a分支输入创建分支的命令，则是在a分支下创建分支

   10. #### git merge：分支合并命令输入git merge a会将a分支合并到主分支![img](https://pic4.zhimg.com/v2-807514785bdbb725053f4e30458bf5f5_1440w.jpg)

      #### 此外，在这里需要注意一点，那就是：在合并分支的时候，要考虑到两个分支是否有冲突，如果有冲突，则不能直接合并，需要先解决冲突；反之，则可以直接合并

   11. #### git branch -d & git branch -D：分支删除命令输入git branch -d a会删除a分支，如果a分支还未合并到主分支则会删除不了，若这时执意要删除则可以用git branch -D进行强制删除

   12. #### git tag：分支添加标签命令（暂时还未理解，之后再补充自己的理解）


# 二，Git与GitHub的绑定

1. ## 生成SSH key

   #### windouws系统没有安装SSH，不过Git Bash应该会自带SSH，在Git Bash中输入ssh检查是否安装SSH，如图则已安装![img](https://pic4.zhimg.com/v2-23abbd2b8bfbc1ae2d2291d3aa6b274f_1440w.jpg)

   #### 接下来输入ssh-keygen -t rsa表示我们指定 RSA 算法生成密钥，然后敲三次回车键，期间不需要输入密码，之后就就会生成两个文件，分别为id_rsa和id_rsa.pub，即密钥id_rsa和公钥id_rsa.pub. 对于这两个文件，其都为隐藏文件,联想笔记本在C:\Users\LEGION\.ssh这个路径

   #### 把公钥id_rsa.pub的内容添加到 GitHub，这样我们本地的密钥id_rsa和 GitHub 上的公钥id_rsa.pub才可以进行匹配，授权成功后，就可以向 GitHub 提交代码

2. ## 添加SSH key

   ![img](https://picx.zhimg.com/v2-d8157e3f5ba22ce64a4bdab14f2c7739_1440w.jpg)

   #### 如上图所示，进入我们的 GitHub 主页，先点击右上角所示的倒三角▽图标，然后再点击Settins，进行设置页面；点击我们的头像亦可直接进入设置页面

   ![img](https://pica.zhimg.com/v2-ea4f291447727e84434b87254a497c12_1440w.jpg)

   #### 如上图所示，进入Settings页面后，再点击SSH and GPG Keys进入此子界面，然后点击New SSH key按钮

   #### ![img](https://pica.zhimg.com/v2-4ef2ed875603194788cf0b99fa975220_1440w.jpg)

3. ## 验证绑定是否成功

#### 在我们添加完SSH key之后，也没有明确的通知告诉我们绑定成功啊！不过我们可以通过在 Git Bash 中输入ssh -T git@github.com进行测试

#### ![img](https://pic2.zhimg.com/v2-aa1938b4970cd5ccddd82406f58aee83_1440w.png)

#### 在我们添加完SSH key之后，也没有明确的通知告诉我们绑定成功啊！不过我们可以通过在 Git Bash 中输入ssh -T git@github.com进行测试

#### 若显示22端口超时，则可以输入vim ~/.ssh/config点击回车后会进入一个新界面此时按格式输入

#### Host github.com

#### Hostname ssh.github.com

#### Port 443

#### 后再按住ESC输入 :wq即可（此处注意:也要输入）

#### 后续可能会有如下情况，这是在确认你是否相信改服务器，输入yes即可
<img width="1015" height="316" alt="屏幕截图 2025-11-07 200250" src="https://github.com/user-attachments/assets/ea7a8533-e92a-45ae-9f64-124d002e512f" />


# 三，通过Git将代码提交到GitHub



1. #### push：该单词直译过来就是“推”的意思，如果我们本地的代码有了更新，为了保持本地与远程的代码同步，我们就需要把本地的代码推到远程的仓库，代码示例

   #### git push origin master

   #### pull：该单词直译过来就是“拉”的意思，如果我们远程仓库的代码有了更新，同样了保持本地与远程的代码同步，我们就需要把远程的代码拉到本地

   #### git pull origin master

2. ## 第一种

   #### 本地没有Git仓库，这时我们就可以直接将远程仓库clone到本地。通过clone命令创建的本地仓库，其本身就是一个 Git 仓库了，不用我们再进行init初始化操作啦，而且自动关联远程仓库。我们只需要在这个仓库进行修改或者添加等操作，然后commit即可
