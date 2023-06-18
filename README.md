# SuperMap iobject-11 Java

## Available classes , will add more in the future
1. com.supermap.analyst.networkanalyst
2. com.supermap.analyst.spatialanalyst
3. com.supermap.data.cloudlicense
4. com.supermap.data
5. com.supermap.data.processing


## Add in your maven project POM
```
<repositories>
    <repository>
        <id>your-project</id>
        <name>your-project</name>
        <url>https://github.com/ismetsk/iobject-java/raw/main/</url>
    </repository>
</repositories>
```

## pack all jars
```
<build>
  <plugins>
    <plugin>
      <artifactId>maven-assembly-plugin</artifactId>
      <configuration>
        <archive>
          <manifest>
            <mainClass>your.package.MainClass</mainClass>
          </manifest>
        </archive>
        <descriptorRefs>
          <descriptorRef>jar-with-dependencies</descriptorRef>
        </descriptorRefs>
      </configuration>
    </plugin>
  </plugins>
</build>
```
```
mvn clean compile assembly:single
```
