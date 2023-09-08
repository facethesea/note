# html css问题



## 1. 去除a标签的下划线

```css
a{
	text-decoration:none;
}
```






## 2. css元素均分宽度

### 2.1 方法一

1.   父元素，子元素 

   ```css
   .father,.son{
       display=flex;
   }
   ```

2.   设置子元素的宽度  = 100%除以子元素数量



### 2.2 方法二

1.  父元素宽度为100%，设置子元素的宽度  = 100%除以子元素数量

​		这种方法，会在子元素间产生空隙——>其原因:html代码中的回车，如:

```html
	<p>123</p>
	<p>321</p>
```

2.  去除空隙

​		2.1 去除回车，如:

```html
	<p>123</p><p>321</p>
```

​		2.2 设置父元素字体大小为0px，子元素字体大小正常

```css
.father{
	font-size:0px;
}
.son{
    font-size:16px;
}
```





## 3. 合并边框

```css
table{
	border-collapse:collapse;
}
```

仅适用于表格table





## 4. 快速创建表格

```html
table>tr>th*5      <!-- th可以换成td -->
```

可以实现:

```html
    <table>
      <tr>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
        <th></th>
      </tr>
    </table>
```





## 5. 元素水平居中

### 5.1 text-align (适用于行内元素)

​	`text-align`	CSS 属性定义行内内容（例如文字）如何相对它的块父元素对齐。`text-align` 并不控制块元素自己的对齐，只控制它的行内内容的对齐。

```css
div{
	text-align:center;         /*	行内内容居中	*/
}
```



### 5.2 块状元素解决方案

```css
div{	
    margin:10px auto;
}
```



### 5.3 多个块状元素解决方案

	1. 将多个块状元素的`display`属性设置为`inline`
	1. 设置父元素的`text-align`为center

```css
.father{
	text-align:center;
}

.son{
    display:inline;
}
```



### 5.4 使用flexbox布局解决多个块状元素

​	使用flex布局，只需要把待处理的块状元素的父元素添加属性`display:flex`及`justify-content:center`

```css
.father{
    display:flex;
    justify-content:center;
}
```





## 6. 元素垂直居中

### 6.1 





## 7. 













# javascript 问题



## 1. 输入

​	`prompt`

```javascript
let a = prompt('请输入:') 		//类似python的input
```

​	变量a默认为string类型,要想转换为number类型，可以:

```javascript
let a = +prompt('请输入:') 
```





## 2. 输出

### 2.1 document.write()

​	用法示例：

​		1.

<img src="C:\Users\Administrator\Pictures\代码\code_1.png" style="zoom: 80%;" />

​			2.



































