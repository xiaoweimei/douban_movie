# douban_movie
[预览地址](https://xiaoweimei.github.io/douban_movie/)
## 2019年2月28日所遇问题
- 影片缩略图无法显示，检查后发现图片请求出现403错误，可能由于referer来源于同一个地方，请求数据过大，而被浏览器直接拦截，后续请求无错
- 解决方法：清除每次请求时携带的referer值(后续看效果)
