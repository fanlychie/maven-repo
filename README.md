<p align="center">
    <a href="#">
        <img src="https://raw.githubusercontent.com/fanlychie/mdimg/master/maven_repo.png">
    </a>
</p>
<p align="center">
    托管的 maven 仓库
</p>

---

## 依赖声明

在 pom.xml 中添加如下配置：


```
<!-- 配置仓库 -->
<repositories>
    <repository>
        <id>fanlychie-maven-repo</id>
        <url>https://raw.github.com/fanlychie/maven-repo/releases</url>
    </repository>
</repositories>
<!-- 配置依赖 -->
<dependencies>
    <dependency>
        <groupId>org.fanlychie</groupId>
        <artifactId>${项目名称}</artifactId>
        <version>${版本号}</version>
    </dependency>
</dependencies>
```

## 构件列表

* beanutils
    - 操纵Java Bean的字段、方法、构造器的工具
* cat-client-mybatis
    - MyBatis接入大众点评CAT监控平台
* cat-dubbo-monitor
    - Dubbo接入大众点评CAT监控平台
* cat-client-dubbo
    - 客户端dubbo接入大众点评CAT监控平台
* commons-codecs
    - 常用编码解码器开发包
* commons-file
    - 文件工具包
* commons-httpclient
    - HTTP 客户端工具包
* commons-httpclient-jdk7
    - HTTP 客户端工具包
* commons-web
    - 常用WEB开发包
* dubbo-devtool
    - Dubbo 服务本地开发调试工具
* jdbc-template-generator
    - 基于 jdbc 和 velocity 实现的模板文件生成器
* jexcel
    - 基于 Apache POI 开发的 Excel 文件读写工具包
* jqrcode
    - 基于 Zxing 开发的二维码图片工具类
* jreflect
    - Java 基础反射操作工具包
* jsp-tag
    - JSP 自定义标签库
* mybatis-template-generator
    - mybatis 模板生成器