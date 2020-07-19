### 1 zadd zrange
```
添加元素
zadd [key] [score] [value] [score] [value] [score] [value]
```
zadd mathScore 99 li 100 hu 80 wang 70 chen

```
查看key中的值，默认按分数从小到大排序
zrange [key] 0 -1  
```
zrange mathScore  0 -1  
```
查看key中的分数和值，默认按分数由小到大排序
zrange [key] 0 -1 withscores
```
zrange mathScore  0 -1 withscores

### 2  zrangebyscore
```
查看局部分数范围内的值
zrangebyscore  [key]  [startScore]  [endScore]
```
zrangebyscore mathScore 90 100

```
查看局部分数范围内的分数和值
zrangebyscore  [key]  [startScore]  [endScore] withscores
```
zrangebyscore mathScore 90 100 withscores

### 3 zrem
```
删除key下分数对应的value
zrem [key] [value]
```
zrem mathScore hu

### 4 zcard zcount zrank zscore
```
获取key中的值长度
zcard [key]
```
zcard mathScore

```
获取指定分数区间的值个数
zcount [key]  [startScore]  [endScore]
```
zcount mathScore 50  80

**排名**
```
获取该值得索引下标
zrank [key] [value]
```
zrank mathScore li

```
获取该值得对应分数
zscore [key] [value]
```
zscore mathScore li
