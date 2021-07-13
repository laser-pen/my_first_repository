1.git init   或者  git 文件夹 init  
初始化一个本地仓库

2.git add （文件，.代表所有未提交的文件）

3.git commit -m “提交备注”
将暂存区的文件提交到本地仓库

4.git remote add origin https://github.com/laser-pen/my_first_repository.git
将本地仓库与一个远程仓库建立连接，origin是远程仓库的名称，一般都叫origin，网址为远程仓库的真实地址

5.git push -u（或 --set-upstream）origin master
推送本地分支到远程主机origin的master分支
如果没有master分支，就创建一个
设置origin为默认主机，以后可以直接git push

6.git remote add Mars https://github.com/laser-pen/my_second_repository.git
将本地仓库与第二个远程仓库建立连接，此时只有一份本地仓库

7.git remote  -v
查看所有的远程仓库地址

8.git push -u Mars master
向远程仓库Mars推送

8.git remote rm Mars
删除远程仓库Mars地址

9.什么是branch
>假设你在写一篇论文。你已经写出了第一个版本，并提交审稿。后来，你获取了新的数据，你正在把你的数据添加到论文中。在这个过程中，审稿人让你改变你的论文的格式。很明显，你不能把你正在更改的版本修改格式后提交给他们。你只想在以前版本基础之上对格式进行修改之后发给他们。
这就是分支背后的思想，Git使这件事情变得非常容易。
注意术语：“branch”和"head"在Git中几乎是同义词，每一个分支都对应一个head，并且每个head代表一个分支。有些时候，"branch"用来指一个head以及在这个head之前的所有commits，而”head“用来指最近一次commit。