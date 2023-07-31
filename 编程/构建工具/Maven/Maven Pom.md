
#Java/Build_Tools
#Maven/Pom

### 通用开头


 以下配置来源  [spring-cloud-alibaba](https://github.com/alibaba/spring-cloud-alibaba/tree/2022.x)

```xml
<!-- 当前 POM 文件遵循的 Maven 模型版本 -->
<modelVersion>4.0.0</modelVersion>
<!-- 当前项目的父项目 -->
<parent>
	<groupId>org.springframework.cloud</groupId>
	<artifactId>spring-cloud-build</artifactId>
	<version>4.0.0</version>
	<relativePath/>
</parent>

<groupId>com.alibaba.cloud</groupId>
<artifactId>spring-cloud-alibaba</artifactId>
<version>${revision}</version>
<packaging>pom</packaging>
<name>Spring Cloud Alibaba</name>
<description>Spring Cloud Alibaba</description>
<url>https://github.com/alibaba/spring-cloud-alibaba</url>
```


### modules \ module

modules 模块集合标签
module 模块标签
```xml
<modules>
	<module>模块名1</module>
	<module>模块名2</module>
</modules>
```


### license

licenses许可证集合标签
license 许可证
```xml
<licenses>  
    <license>        
	    <name>Apache License, Version 2.0</name>  
        <url>https://www.apache.org/licenses/LICENSE-2.0.txt</url>  
        <distribution>repo</distribution>  
    </license>
</licenses>

```

### scm 

版本管理与发布

以下配置来源  [spring-cloud-alibaba](https://github.com/alibaba/spring-cloud-alibaba/tree/2022.x)
```xml
<scm>
	<url>https://github.com/alibaba/spring-cloud-alibaba</url>
	<connection>
		scm:git:git://github.com/alibaba/spring-cloud-alibaba.git
	</connection>
	<developerConnection>
		scm:git:ssh://git@github.com/alibaba/spring-cloud-alibaba.git
	</developerConnection>
	<tag>HEAD</tag>
</scm>

```

### properties 

属性定义


通过${属性名} 使用
```xml
<properties>
	<属性名>属性值</属性名>
</properties>
```


### dependencyManagement 

依赖管理

通常定义在父类的pom中，并在子模块的 POM 文件中进行继承和覆盖。可以确保所有子模块使用相同的依赖版本，避免版本冲突和不一致性。简化了对依赖版本的管理和维护。

```xml
<dependencyManagement>
  <dependencies>
    <dependency>
      <groupId>org.example</groupId>
      <artifactId>example-artifact</artifactId>
      <version>1.0.0</version>
    </dependency>
    <!-- 其他依赖 -->
  </dependencies>
</dependencyManagement>
```



### developers \ developer

开发人员名单

```xml
<developers>
	<developer>
		<name>developer_name</name>
		<email>developer_email</email>
	</developer>
</developers>        
```


