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