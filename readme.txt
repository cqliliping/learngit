
GitHub需要SSH Key，Gitee也需要， 用来识别是你推送的内容，Github 和 Gitee还可以添加多个SSH Key
git bash在本地建立了一个版本库，GitHub是一个远程库，两者进行远程同步
关联远程库   删除远程库 注意这里的删除是删除本地库与远程库的联系，删除远程库需要得到Github后台页面进行删除
不能在同一目录下面存在多个.git文件夹

Creating a new branch is quick
我学会git分支啦
分支李丽平
要先git bash切换所在分支，push的分支才能上传到对应分支下面
如果在git bash创建一个分支，然后直接push到git，网页版会自动生成么
答案是会自动生成，不过要牢记git push要切换到当前.git文件夹内才能上传到当前分支
del/llp分支是git bash建立的，创建后会删除，删除会同步到远程库么，
是不是git bash只是删除自己的del/llp，删除需要远程库也删除当前分支 正解
git clone支持不指定分支和指定分支
还有一个很好理解的点就是：git push要在当前.git同一文件夹。git clone的文件夹是.git的目文件夹，要切换到
下级目录才能push

所以一般目前的工作就是在一个文件夹内clone std C1001 等文件下来，修改调试后在push上去（当然要是自己的分支）
像C1204 C1264就需要先建立远程库，自己创建分支，修改后再上传修改的内容。没有远程库，只有本地库就没有联系
无法知道上传到哪里，甚至没有C1204等的远程库也可以
通常来说本地库有本地库的操作，远程库有远程库的操作，本地可能有多个branch，但是不能在同一文件夹从远程库pull
多个branch只能pull一个，本地库的多个branch可以本地merge，远程库的branch也可以GitHub后台merge
后台将branch merge 到 master有一系列操作，解决冲突，同意合并，安全删除分支，然后分支有了新的修改再上传
本地merge和远程库merge类似，只是命令行和GUI操作

又来复盘了，因为标准表直接修改usr_config.h即可，定制表才需要建立新的工程，所以直接在Git远程库建立分支
（以最新的雷主任代码为模板，后面自己在更新代码同时会将雷主任的merge到自己代码，也可以自己代码merge到master）
建立自己的dev/lilp分支后，git bash在文件夹中clone 该分支，然后根据需求修改代码，然后push到自己的分支，这是
第一阶段最基础的使用方法