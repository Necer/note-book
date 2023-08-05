
风格检查

#Java/Build_Tools
#Maven/Plugin 
#Code/Check

### 配置样本

```xml
<plugin>  
    <groupId>org.apache.maven.plugins</groupId>  
    <artifactId>maven-checkstyle-plugin</artifactId>  
    <version>${maven.checkstyle.version}</version>  
    <executions>        
	    <execution>            
		    <id>checkstyle-validation</id>  
			<phase>validate</phase>  
            <goals>                
	            <goal>check</goal>  
            </goals>            
		    <configuration>                
			    <configLocation>
				    <!-- 项目根目录能解析到的 -->
				    checkstyle.xml
			    </configLocation>  
                <suppressionsLocation>
		            <!-- 项目根目录能解析到的 -->
	                checkstyle-suppressions.xml
				</suppressionsLocation>  
                <includeTestSourceDirectory>true</includeTestSourceDirectory>  
                <consoleOutput>true</consoleOutput>  
                <failsOnError>true</failsOnError>  
                <failOnViolation>true</failOnViolation>  
                <violationSeverity>warning</violationSeverity>  
            </configuration>       
		 </execution>    
	 </executions>
</plugin>
```


