## 获取依赖的方式

- [x] ***pom.xml*** **（此方式每次都需要配置 repository）**

在 pom.xml 中添加如下配置：


```
<repositories>
    <repository>
        <id>github-maven-repo</id>
        <url>https://raw.github.com/fanlychie/maven-repo/releases</url>
    </repository>
</repositories>

<dependencies>
    <dependency>
        <groupId>org.fanlychie</groupId>
        <artifactId>${项目名称}</artifactId>
        <version>${版本号}</version>
    </dependency>
</dependencies>
```

- [x] ***settings.xml*** **（此方式仅需配置一次 repository）**

在 settings.xml 中添加如下配置：


```
<profiles>
    <profile>
        <id>development</id>
        <repositories>
            <repository>
                <id>github-maven-repo</id>
                <url>https://raw.github.com/fanlychie/maven-repo/releases</url>
            </repository>
        </repositories>
    </profile>
</profiles>

<activeProfiles>
    <activeProfile>development</activeProfile>
</activeProfiles>
```

在 pom.xml 中添加如下配置：


```
<dependencies>
    <dependency>
        <groupId>org.fanlychie</groupId>
        <artifactId>${项目名称}</artifactId>
        <version>${版本号}</version>
    </dependency>
</dependencies>
```

## 获取源码的方式

在项目中引入依赖包后，右键项目 —> Run As —> Maven build... —> Goals 栏键入 dependency:sources —> Run