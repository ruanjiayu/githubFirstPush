# githubFirstPush
第一次提交到github仓库的步骤以及遇到的问题

---
### 当你本地已经存在代码的情况下，使用下面的方式来提交代码
1. 在本地使用git init
2. git remote add origin https://github.com/xxx
3. git pull origin master
4. git add .
5. git push -u origin master

### 当你在github上提前先创建好了库


### 问题
##### 1. git commit提交修改好的文件时候，提示`Changes not staged for commit`
- 使用`git status` 来查看本地修改好的文件是否已将放入暂存区
- 如果发现没有加入暂存区，那么你可以使用`git add .`或者 `git add fileName`来加入暂存区
- 最后你可以使用`git commit -m "xxxxx"`来提交暂存区的数据到本地库，当然你可以直接可以使用`git commit -am "xxxx""`来进行直接的提交

##### 2. 已经加入暂存区的文件如何撤回，保留工作区内的文件
- 使用`git rm --cached fileName` 可以撤回相对应的文件。
- 使用`git rm -r --cached .` 可以撤回所有的文件
##### 3. 删除工作区内的文件,并且进行提交上传。注意:要删除的文件是没有修改过的，就是说和当前版本库文件的内容相同
- 使用`git rm fileName`，可以删除工作区内的文件,并且加入到暂存
- 使用`git commit -m "xxxxxx"`将删除了的文件提交到暂存区
##### 4. 强制删除工作区和暂存区内对应的文件，并将删除好后的状态提交到暂存区
- 使用`git rm -f fileName`,可以删除工作区内的文件,并且加入到暂存区





