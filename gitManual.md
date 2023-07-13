# Git Manual
****
### 在本地初始化仓库

1. 进入项目目录 `cd /e/git-workspace/markdown-learn`
2. 执行 `git init` 初始化仓库，该命令将创建一个名为 .git 的子目录，这个子目录含有你初始化的 Git 仓库中所有的必须文件。
3. 执行 `git add <files>` 该命令使用文件或目录的路径作为参数，如果参数是目录的路径，该命令将递归地跟踪该目录下的所有文件。
这是个多功能命令：可以用它开始跟踪新文件，或者把已跟踪的文件放到暂存区，还能用于合并时把有冲突的文件标记为已解决状态等。
4. `git commit -m '提交信息'` 该命令将放在暂存区域的快照提交到 Git 仓库中。
`git commit -a -m '提交信息'` 该命令就会自动把所有已经跟踪过的文件暂存起来一并提交，从而跳过 git add 步骤。


### 克隆远程仓库

- 执行`git clone <url>` 命令克隆远程仓库，例如执行`git clone https://github.com/caogaoliang/markdown-learn.git`，可通过额外的参数自定义本地仓库的名字：`git clone <url> [newname]`
- 无需再进行 `git init` 初始化仓库了
- 执行 `git add <files>` 和  `git commit -m '提交信息'` 
- `git push origin master` 将本地仓库的内容push到远程仓库，在第一次向远程仓库提交代码的时候，需要输入账号及密码进行验证

- `git remote add <remote-name> <remote-url>` 其中 `<remote-name>` 为远程仓库设置的名称，`<remote-url>` 为远程仓库的 URL ，如：`git remote add origin-cgl https://gitee.com/cao-gaoliang/hospital-guide-mini-manager.git`，通过这种方式可以绑定**多个远程仓库**。
- 通过`git remote` 查看已添加的远程仓库
- `git push <remote-name> <branch-name>` 通过指定 `<remote-name>` 即远程仓库的名字，将更改推送到指定的仓库。如：`git push origin-cgl master`



### 检查当前文件状态

- `git status` 命令可以查看哪些文件处于什么状态。


### 配合 Github 使用

1. 创建github仓库: 在 [github网站](https://github.com/caogaoliang) 创建仓库(Create repository)
2. 在本地创建项目目录，以项目目录为 Git 仓库，打开 Git Bash 的命令行窗口
3. 使用`git init`命令初始化 Git 仓库，在我们初始化仓库之后，项目目录就成为了一个 Git 仓库，并且默认进入 Git 仓库的 master 分支
4. 使用`git remote add markdown-origin https://github.com/caogaoliang/markdown-learn.gits`命令，关联远程仓库，其中markdown-origin为远程仓库的名字
5. 使用`git pull markdown-origin main`命令同步远程仓库和本地仓库
6. 使用`git add <file>`，该命令并没有把文件提交到 Git 仓库，而是把文件添加到了临时缓冲区，有效防止了我们错误提交的可能性。
7. 输入`git commit -m "提交信息"`命令，将文件提交到 Git 仓库，-m表示提交信息，提交信息写在双引号内
8. 使用`git push markdown-origin master`命令将将本地仓库修改（或者添加）的内容提交到远程仓库
9. 输入`git status`命令，查看仓库的状态


### 查看已暂存和未暂存的修改 git diff

- 不加参数直接输入 `git diff` ，此命令比较的是工作目录中当前文件和暂存区域快照之间的差异。输入 `q` 退出。
- `git diff --staged` 这条命令将比对已暂存文件与最后一次提交的文件差异。


### 获取帮助 help

- `git <verb> --help` 可获取 Git 命令的综合手册，例如执行 `git add --help` 可以获得 `git add` 命令的综合手册。
-  `git <verb> -h` 可以用 -h 选项获得更简明的 “help” 输出，例如执行 `git add -h`


