
代码覆盖率插件

#Java/Build_Tools
#Maven/Plugin
#Code/Check 

## JaCoCo 插件 

[[JaCoCo]]

引入参考
```xml
<build>  
    <plugins>
		<plugin>
			<groupId>org.jacoco</groupId>  
            <artifactId>jacoco-maven-plugin</artifactId>  
            <version>${jacoco.version}</version>  
            <executions> 
			    <execution>
	                <id>jacoco-initialize</id>  
                    <goals>                       
	                    <goal>prepare-agent</goal>  
                    </goals>               
				</execution>               
				<execution>                   
					<id>jacoco-site</id>  
		            <phase>test</phase>  
                    <goals>                        
	                    <goal>report</goal>  
                    </goals>                
	            </execution>           
			</executions>        
		</plugin>    
	</plugins>
</build>
```
