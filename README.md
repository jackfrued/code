# Git演示项目

2018年6月22日

- `git init`
- `git add <filename1> <filename2>`
- `git add .`
- `git checkout -- <filename>`
- `git checkout -- .`
- `git status`
- `git config --global user.name <username>`
- `git config --global user.email <email>`
- `git commit -m 'reason'`
- `git log`
- `git reset --hard HEAD^`
- `git reset --hard <version>`

- `git remote add origin <url>`
- `git push -u origin <branch>`
- `git pull`


1. 克隆项目到本地
```git clone <url>```
  
2. 创建并切换到自己的分支
```git branch jack```
```git checkout jack```
或
```git checkout -b jack```

3. 在自己的分支上做开发然后实施版本控制
```git add .```
```git commit -m 'reason'```

4. 将自己的工作合并到master上 
```git checkout master```
```git merge jack```
如果不希望使用fast-forward方式合并（git log中没有分支记录）
```git merge --no-ff jack -m 'reason'```

5. 如果想通过图形化的方式查看到分支信息
```git log --graph --pretty=oneline --abbrev-commit```
