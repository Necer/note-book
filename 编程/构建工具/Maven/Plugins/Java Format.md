
代码格式
#Java/Build_Tools
#Maven/Plugin 
#Code/Format

### spring-javaformat-maven-plugin


引入参考
```xml
<build>
  <plugins>
    <plugin>
      <groupId>io.spring.javaformat</groupId>
      <artifactId>spring-javaformat-maven-plugin</artifactId>
      <version>0.0.6</version>
      <configuration>
        <skip>false</skip>
      </configuration>
      <executions>
        <execution>
          <id>format</id>
          <phase>verify</phase>
          <goals>
            <goal>apply</goal>
          </goals>
        </execution>
      </executions>
    </plugin>
  </plugins>
</build>
```

