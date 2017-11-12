## 当前目录中查找含有 ls 的文件
```plain
grep "ls" -r .
```

## 高亮命中的内容
```plain
grep --color=auto "ls" -r .
```

## 高亮命中的内容，并给出行号
```plain
grep --color=auto "ls" -n -r .
```

## 高亮命中的内容，并给出行号
```plain
grep --exclude-dir={.bzr,CVS,.git,.hg,.svn,node_modules} "ls" -n -r .  
```