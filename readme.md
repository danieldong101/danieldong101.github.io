1. 首页的分页显示，跳过了开头的4篇文章，如果不要这个功能的话，也就是不要跳过文章，需要怎么做？只需要在theme.css文件里进行如下更改。
```
.homefirstpage .main-loop .main-loop-card:nth-child(-n+5) {
	display:none !important;
}
```
改成
```
.homefirstpage .main-loop .main-loop-card:nth-child(-n+1) {
	display:none !important;
}
```