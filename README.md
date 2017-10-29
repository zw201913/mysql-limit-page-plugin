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
