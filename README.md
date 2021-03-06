基于SpringMVC, Spring (Version 4.2.3) + MyBatis (Version 3.2.2) 的API应用
适合APP后端接口, 小程序后端接口, 前后端分离的接口支持.

开发环境:
Apache Maven 3.3.3 + JDK 8 + MySQL 5.7 + Tomcat 8 

支持以下特性:
1. 使用Maven 搭建整个环境, 开发环境和线上环境使用maven 环境变量区分开; pom.xml
2. 全局使用JSON 序列化返回, 返回文本;
3. 多数据源配置, 用户库表 ssm2user + 商品库表 ssm2product
4. 使用MyBatis 的SQL注解开发DAO层, @Select, @Insert, @Update等 (个人偏好注解SQL, 和DAO放在一起)
5. 配置HiException, 配置全局的异常拦截器, 基于 HandlerExceptionResolver
6. 配置全局的自定义注解拦截器, 验证客户端上传参数合法性, 基于 HandlerInterceptorAdapter
7. 配置部署脚本, 分别部署开发和线上环境

后续优化:
1. 基于注解的AOP缓存
2. 国际化 i18n

一些命令:
1. mvn eclipse:eclipse   #初始化工程
2. mvn dependency:sources  #下载依赖Jar包源码
3. mvn clean install -P develop  #本地打开发环境war包
4. mvn clean install -P production  #本地打线上环境war包


EMail联系方式: greatwqs#163.com