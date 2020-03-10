git命令
1.创建一个空目录 
mkdir 文件名learngit
2.进入文件
cd learngit
3.显示当前目录
pwd
4.创建可管理的仓库版本库，自动为我们创建了唯一一个master分支
git init
5.添加修改文件
git add . 或git add 文件名 文件名（如readme.txt）
6.文件提交仓库
git commit -m "本次提交的说明"
7.仓库当前的状态
git status
8.查看具体修改了什么内容
git diff
9.显示从最近到最远的提交日志
git log
10.提交日志时间线
git log --pretty=oneline
11.回退版本  在Git中，用HEAD表示当前版本，上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100
git reset --hard HEAD^
12.要重返未来，查看命令历史，以便确定要回到未来的哪个版本
git reflog
13.Git允许我们在版本的历史之间穿梭，回退或重返某个版本，根据命令历史或提交历史查找id，使用前5位也可
git reset --hard commit_id(如4b468)
14.查看工作区和版本库里面最新版本的区别
git diff HEAD -- readme.txt