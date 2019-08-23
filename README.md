# douban_movie
[预览地址](https://xiaoweimei.github.io/douban_movie/douban_movie.html)
## 2019年2月28日所遇问题
- 搜素按钮点击可以用，文本框输入直接按回车不起作用。
- 解决方法，先在input里面绑定了回车触发点击事件，然后发现form表单有bug还不知道如何解决，删除form标签后一切回归正常
- 影片缩略图无法显示，检查后发现图片请求出现403错误，可能由于referer来源于同一个地方，请求数据过大，而被浏览器直接拦截，后续请求无错
- 解决方法：清除每次请求时携带的referer值(后续看效果)
- 采用了https://github.com/LingYanSi/blog/issues/89
## 2019年8月8日所遇问题
- 豆瓣api https://api.douban.com挂掉
- 解决方法，换用新的api https://douban.uieee.com
## 2019年8月21日所遇问题
- 查询功能报错，出现404及`Provisional headers are shown`，具体等详细排查
- api挂掉了我也没办法
