<h2>Kylinsky Lab</h2>
[Community of Kylinsky](localhost:8081):

Kylinsky Lab网站，旨在为实验室同学提供在线学习和交流的平台
Email:648376320@qq.com

<h2>相关网站</h2>
[springboot API](https://spring.io/guides)

[Spring Web Doc](https://spring.io/guides/gs/serving-web-content/)

[BootStrap Doc](https://v3.bootcss.com/getting-started/)

[GitHub OAuth Doc](https://docs.github.com/en/developers/apps/creating-an-oauth-app)

<h2>工具</h2>
[Visual Paradigm](https://www.visual-paradigm.com/cn/)

[okhttp Web](https://square.github.io/okhttp/)

[mvnrepository:即mvn仓库](https://mvnrepository.com/)


<h2>一些项目上的更新</h2>
在GithubProvider.java文件中，获取用户名的代码段，需要更改为入下所示：
```
Request request = new Request.Builder()
.url("https://api.github.com/user")
.header("Authorization","token "+accessToken) 
.build();
```
是因为GitHub改版了，需要从 header 里面传递，“token后面有个空格”。
[具体参考点击此处](https://docs.github.com/en/free-pro-team@latest/rest/overview/other-authentication-methods)


