## 查看某个commit的改动
```plain
git show <commit>
```

## 查看每一行是谁改的
```plain
git blame <filepath>
```

## 删除文件（从 git repo 中删除，同时物理删除）
```plain
git rm file.txt
```

## 删除文件（从 git repo 中删除，但是不物理删除）
```plain
git rm --cached file.txt
```

## 设置默认编辑器为 vim
```plain	
git config --global core.editor vim
```