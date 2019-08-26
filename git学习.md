##创建git文件夹
	``mkdir fliename//创建文件夹
	cd fliename//进入文件夹
	pwd//显示文件夹
	git init //把当前文件夹变成git库
##提交文件
	git add fliename//添加文件
	git commit -m "注释"//提交添加的文件
##检查文件
	git status//检查文件是否修改
	git diff //查看文件修改了什么
	git log //查看提交日志
	git log --pretty=oneline //简化日志
	git reflog //查看历史日志
##改文件
	git reset --hard HEAD^ //回退到上一次的提交，两个^^就是上上个版本
	git reset --hard 提交id // 到id的位置
	git checkout -- fliename //当文件没有提交前可以把工作区的修改全部撤销
	//总之，就是让这个文件回到最近一次git commit或git add时的状态。
	用命令git reset HEAD <file>可以把暂存区的修改撤销掉（unstage）
##删除文件
	rm <flie>//删除文件
	//如果是删错了，但版本库里没有删
	git checkout -- <flie>

	//在版本库中删除文件
	git rm <flie>
	git commit -m "remove test.txt"

