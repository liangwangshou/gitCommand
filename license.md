<div style="border: 1px solid black;">
        <h3 style="color: red;">版本回退</h3>
        <h4>git log 显示最近到最远的提交日志</h4>
        <h4>cat "filename" 查看指定文件的内容</h4>
        <h4>git reflog 记录每一次的命令</h4>
        <h4>HEAD指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令git reset --hard commit_id。</h4>
</div>
    <p>
        $ git reset --hard HEAD^ 回到上一个版本 <br> --hard参数有啥意义？这个后面再讲，现在你先放心使用。<br>
        上一个版本就是HEAD^，上上一个版本就是HEAD^^，当然往上100个版本写100个^比较容易数不过来，所以写成HEAD~100
    </p>
    <p>
        $ git reset --hard "xxx" 网上寻找回退版本前的该版本的版本号
    </p>
     <h4>git status 查看文件的状态 包括工作区，版本库中stage暂存区和提交分支的时候文件的不同情况</h4>
    <h4>git checkout -- readme.txt 把readme.txt文件在工作区的修改全部撤销</h4>
    <p>命令git checkout -- readme.txt意思就是，把readme.txt文件在工作区的修改全部撤销，这里有两种情况：

        一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；

        一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。</p>
    <p>
        要关联一个远程库，使用命令git remote add origin git@server-name:path/repo-name.git；

        关联后，使用命令git push -u origin master第一次推送master分支的所有内容；

        此后，每次本地提交后，只要有必要，就可以使用命令git push origin master推送最新修改；
    </p>
    
