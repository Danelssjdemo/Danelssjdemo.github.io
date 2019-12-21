# 输出为静态网站

你有两种方式输出一个静态的网站：

# 本地预览是自动生成

当你编辑好 gitbook 文档之后，你可以使用 gitbook 的命令来进行本地预览。

$ gitbook serve ./{book_name}
gitbook会启动一个4000端口用于预览。

比如，通过gitbook serve来预览本文档：

$ gitbook serve gitbook-howtouse

Press CTRL+C to quit ...

Live reload server started on port: 35729
Starting build ...
Successfully built!

Starting server ...
Serving book on http://localhost:4000
你可以你的浏览器中打开这个网址： http://localhost:4000