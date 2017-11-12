该命令用于对图像进行处理。

## 安装
ubuntu: 
```plain
$ sudo  apt-get install imagemagick  
```

## 批量转换格式
```plain
for i in *.png
do
    convert $i `basename $i .png`.jpg
done
```

## 修改图片大小
下面两个方式都不会导致图片被裁剪。

方式1：
```plain
convert -resize 50%x50% 01.jpg 01-small.jpg
```
如果是 50%x10%，图像会被压扁。

方式2：
```plain
convert -resize 800x600 01.jpg 01-small.jpg
```
长和宽有一个达到即可。例如原图大小是1600x1052，最终结果是800x526大小。


## 调整图片存储大小
```plain
convert  -quality 60 01.jpg 01-storage-small.jpg
```
注意，图片质量会下降。