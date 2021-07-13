1.寻找指定目录下最大深度文件夹内的文件并删除这些文件:

```
find ./ -maxdepth 3 -type d -name "system" -exec rm -rf {} \;
```

maxdepth,指定查找的最大深度;

type,指定文件类型,d代表目录；

name,指定文件名字；

exec,执行bash命令.exec把find到的文件名作为参数传递给后面的命令行，代替{}的部分.exec 必须由一个 ; 结束，而因为通常 shell 都会对 ; 进行处理，所以用 \; 防止这种情况

