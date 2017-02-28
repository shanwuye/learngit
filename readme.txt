here is a new text;
now i wanna add this line let's get longer;
third line;
creating a new branch is quick;
查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>

创建+切换分支：git checkout -b <name>

合并某分支到当前分支：git merge <name>

删除分支：git branch -d <name>

$ git merge --no-ff -m "merge with no-ff" dev    (dev 准备合并dev分支，请注意--no-ff参数，表示禁用Fast forward,如果要强制禁用Fast forward模式，Git就会在merge时生成一个新的commit，这样，从分支历史上就可以看出分支信息。合并分支时，加上--no-ff参数就可以用普通模式合并，合并后的历史有分支，能看出来曾经做过合并，而fast forward合并就看不出来曾经做过合并。)

$ git log --graph --pretty=oneline --abbrev-commit  (用git log --graph命令可以看到分支合并图。)
