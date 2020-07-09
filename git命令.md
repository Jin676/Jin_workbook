### 使用 vscode 操作 git
    1. 创建 **本地仓库** 和 **远程仓库**
       * 创建远程库
       * 本地仓库要有.gitignore文件(没有就自己创建)，被忽略的文件
       * git init 初始化本地仓库
       * git add .xx 添加文件到暂存区
       * git commit -m "init app"  将暂存区文件提交到版本区,""里面是你起的名字
       注意：/node_modules 代表根目录下的，你要放入仓库的文件
             node_modules 不加xxx则代表根目录及其子目录下的所有文件
    2. 将本地仓库代码**推送**到远程
       *  git remote add origin https://github.com/Jin676/Jin_workbook.git
       *  git push origin master 本地推送到远程 创建了master分支
       *  创建新分支 git checkout -b xxxx  （xx是创建或者切换的分支）
       *  将新分支推送到远程git push origin dev
       注意： 如果要账号和密码，网上搜索
    3. 如果**本地有变化**，推送到远程
       * git add .
       * git commit -m "updata xxx"
       * git push origin dev
    4. **远程有变化**，拉取到本地
       * git pull origin master (master/或者dev都行)
    5. 新员工克隆远程仓库到本地
       git clone 地址.git就可以 (目前只有master分支)
       git checkout -b dev origin/dev (不是将远程dev分支拉取到本地，而是克隆时候已经下载了，而没有创建分支)
     常见命令：
     git branch 查找分支
     git checkout dev 切换分支
-----------------------------------------------
   