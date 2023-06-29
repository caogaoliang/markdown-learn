## git manual

1. 创建github仓库: 在 [github网站](https://github.com/caogaoliang) 创建仓库(Create repository)
2. 在本地创建项目目录，以项目目录为 Git 仓库，打开Git Bash的命令行窗口
3. 使用`git init`命令初始化 Git 仓库，在我们初始化仓库之后，项目目录就成为了一个 Git 仓库，并且默认进入 Git 仓库的 master 分支
4. 使用`git remote add markdown-origin https://github.com/caogaoliang/markdown-learn.gits`命令，关联远程仓库，其中markdown-origin为远程仓库的名字
5. 使用`git pull markdown-origin main`命令同步远程仓库和本地仓库
6. 使用`git add <file>`，该命令并没有把文件提交到 Git 仓库，而是把文件添加到了临时缓冲区，有效防止了我们错误提交的可能性。
7. 输入`git commit -m "提交信息"`命令，将文件提交到 Git 仓库，-m表示提交信息，提交信息写在双引号内
8. 使用`git push markdown-origin master`命令将将本地仓库修改（或者添加）的内容提交到远程仓库
9. 输入`git status`命令，查看仓库的状态
