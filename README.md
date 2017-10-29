# mysql-limit-page-plugin
mybatis generator分页插件



第一步:把pom.xml中配置maven插件


    <plugin>
        <groupId>org.mybatis.generator</groupId>
        <artifactId>mybatis-generator-maven-plugin</artifactId>
        <version>1.3.5</version>
        <configuration>
            <verbose>true</verbose>
            <overwrite>true</overwrite>
        </configuration>
        <dependencies>
            <dependency>
                <groupId>mysql</groupId>
                <artifactId>mysql-connector-java</artifactId>
                <version>5.1.41</version>
            </dependency>
            <dependency>
                <groupId>com.github.zw201913</groupId>
                <artifactId>mysql-limit-page-plugin</artifactId>
                <version>1.0.1</version>
            </dependency>
         </dependencies>
     </plugin>


第二步:添加generatorConfig.xml配置文件


    1.下载或拷贝 https://github.com/zw201913/mysql-limit-page-plugin/tree/master/src/main/resources 里面的generatorConfig.xml配置文件
    
    
    2.将配置文件放在src/main/resources下面,名字要保持一致
    
    
    3.按照mybatis generator的规范修改里面的generatorConfig.xml,使配置文件符合自身项目的实际情况
    
    
    4.配置完毕后，使用maven命令  mybatis-generator:generate  即可自动生成mybatis分页代码
