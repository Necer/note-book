


### modules \ module

modules 模块集标签
module 模块标签，归属于modules
```xml
<modules>
	<module>模块名1</module>
	<module>模块名2</module>
</modules>
```


### license

许可证
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
