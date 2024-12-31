> #### 作者主页：[舒克日记](https://blog.csdn.net/cativen)
>
>  简介：Java领域优质创作者、Java项目、学习资料、技术互助
>
> <b><font color=red>文中获取源码</font></b>

# 项目介绍

使用网上手机商城的用户分管理员和用户两个角色的权限子模块。

​

管理员所能使用的功能主要有：主页、个人中心、用户管理、商品分类管理、商品信息管理、系统管理、订单管理等。

用户可以实现主页、个人中心、我的收藏管理、订单管理等。

前台首页可以实现商品信息、新闻资讯、我的、跳转到后台、购物车等。

# 环境要求

1.运行环境：最好是java jdk1.8,我们在这个平台上运行的。其他版本理论上也可以。

2.IDE环境：IDEA,Eclipse,Myeclipse都可以。推荐IDEA;

3.tomcat环境：Tomcat7.x,8.X,9.x版本均可

4.硬件环境：windows7/8/10 4G内存以上；或者Mac OS;

5.是否Maven项目：是；查看源码目录中是否包含pom.xml;若包含，则为maven项目，否则为非maven.项目

6.数据库：MySql5.7/8.0等版本均可；

# 技术栈

运行环境：jdk8 + tomcat9 + mysql5.7 + windows10

服务端技术：Java、Spring、SpringMVC、Mybatis，SSM

前端：jsp

# 使用说明

1.使用Navicati或者其它工具，在mysql中创建对应sq文件名称的数据库，并导入项目的sql文件；

2.使用IDEA/Eclipse/MyEclipse导入项目，修改配置，运行项目；

3.将项目中config-propertiesi配置文件中的数据库配置改为自己的配置，然后运行；

# 运行指导

idea导入源码空间站顶目教程说明(Vindows版)-ssm篇：

http://mtw.so/5MHvZq

源码地址：[http://www.codegym.top](http://www.codegym.top/)


# 运行截图

## 功能模块截图

![image20241130113001714](https://i-blog.csdnimg.cn/img_convert/93f579214080ff96cc610074531aaafa.png)

### 项目截图

前台

![ssm109基于jsp的网上手机商城jsp0](https://i-blog.csdnimg.cn/img_convert/1642ad27cc6bf0270c20eb54f4fb7882.png)

![ssm109基于jsp的网上手机商城jsp1](https://i-blog.csdnimg.cn/img_convert/5a77a5a8840de6e07c7cc1e7cae5c298.png)

![ssm109基于jsp的网上手机商城jsp2](https://i-blog.csdnimg.cn/img_convert/94988a915e3866e12d9885c643108198.png)

后台

![ssm109基于jsp的网上手机商城jsp3](https://i-blog.csdnimg.cn/img_convert/52fb9a830fe9a358b01160b2a36fc34b.png)

![ssm109基于jsp的网上手机商城jsp4](https://i-blog.csdnimg.cn/img_convert/24db84779686ba866f92e71f449a0bfe.png)

![ssm109基于jsp的网上手机商城jsp5](https://i-blog.csdnimg.cn/img_convert/89525cdb65a856fc517b4d81831e685c.png)

![ssm109基于jsp的网上手机商城jsp6](https://i-blog.csdnimg.cn/img_convert/d1bdd0539d41487c22bc0f6472fc21f1.png)

![ssm109基于jsp的网上手机商城jsp7](https://i-blog.csdnimg.cn/img_convert/0f09d192518d13ae32a75ddab8f6158e.png)
### 代码

```
    @Operation(summary = "通用webhook")
    @PostMapping("/common")
    @LogRecord
    public SingleResponse<Boolean> commonWebhook(@RequestBody JSONObject params) {

        return SingleResponse.of(true);
    }
```
