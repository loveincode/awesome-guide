```
查看进程数
pstree -p | wc -l 查整个系统的进程数

pstree -p [pid] | wc -l 查看进程的线程数

top -H -p [pid]

cat /proc/[pid]/status
```


awk命令 文本分析 https://www.jianshu.com/p/47f9c67daa63
