## 如何禁止chrome浏览器http自动转成https
### Chrome/Opera 浏览器
1. 地址栏中输入 chrome://net-internals/#hsts
2. 在 Delete domain security policies 中输入项目的域名，并 Delete 删除
3. 可以在 Query HSTS/PKP domain 测试是否删除成功

### Safari 浏览器
1. 完全关闭 Safari
2. 删除 ~/Library/Cookies/HSTS.plist 这个文件
3. 重新打开 Safari 即可
4. 极少数情况下，需要重启系统

### Firefox 浏览器
1. 关闭所有已打开的页面
2. 清空历史记录和缓存
3. 地址栏输入 about:permissions
4. 搜索项目域名，并点击 Forget About This Site
