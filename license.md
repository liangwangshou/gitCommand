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
