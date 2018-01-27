# 一级标题
## 二级标题
### 三级标题
#### 四级标题

## 段落
哈喽，大家好，我是梁佳鹏  
我今年18  
我是**粗体**  
我是*斜体*  
我是***加粗斜体***  
我是~~删除~~  
无序列表  

- 一级  
    - 二级  
        - 三级  
    
- 一级

有序列表

1. abc  
    1. abc  
2. cde  

## 链接  
- 外部链接: [百度](http://www.baidu.com)
- 内部连接: [代码块](README.md#代码块)  
- 引用连接写法1: [百度]  
- 引用连接写法2: [百度][baidu] 

[百度]: http://www.baidu.com
[baidu]: http://www.baidu.com

## 图片  
- 外部调用:  
![无显示替换文本](http://img.zcool.cn/community/01690955496f930000019ae92f3a4e.jpg@2o.jpg "鼠标悬停显示")  
![无显示替换文本](https://www.baidu.com/img/bd_logo1.png "鼠标悬停显示")  
- 内部调用:  
![无显示替换文本,可为空](./test.jpg "鼠标悬停显示")  
- 引用连接写法1:  
![无显示替换文本][图片1]

[图片1]: https://www.baidu.com/img/bd_logo1.png




## 引用  
>这是一个引用

>>这是第二次引用

## 代码块  

shell声明一个变量为`abc=1`,输出一个变量为`echo ${abc}`
```bash
#!/bin/bash
for a in `cat a.txt`
do
    akey=`echo ${a}|awk -F "," {'print $1'}`
    avalue=`echo ${a}|awk -F "," {'print $2'}`
    for b in `cat b.txt`
    do
        bkey=`echo ${b} |awk -F "," {'print $1'}`
        bvalue=`echo ${b} |awk -F "," {'print $2'}`
        if [ ${bkey} == ${akey} ]
        then
            if [ ${avalue} == ${bvalue} ]
            then
                echo ${akey},${avalue} >>c.txt
            fi
        fi
    done
done
    echo ${akey} >>c.txt
    echo ${bkey} >>c.txt
```


