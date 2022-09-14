## Typora-to-bilibili-configuration

插件来源：[typora-plugin-bilibili: Typora粘贴图片自动上传到Bilibili图床](https://github.com/xlzy520/typora-plugin-bilibili)

bilibili部分：登录B站 -> F12打开开发者工具 -> 应用程序 -> Cookies -> SESSDATA，复制

![bilibili部分](bilibili部分.png)

Typora部分：文件->偏好设置->插入图片时【上传图片】-上传服务【Custom Command】->命令【exe绝对路径 token=SESSDATA 】->验证图片上传选项

![typora部分](typora部分.png)

防盗链部分：B站外链直接引用到自己网站上无法成功加载

> "B站的防盗链，利用的是HTTP的Referer属性做判断。如果Referer是他白名单之外的网站，就会返回403。"

只需要在页面的`<head>`标签下添加代码：

		<meta name="referrer" content="no-referrer">