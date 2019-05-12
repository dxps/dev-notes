## Apache Maven - Notes

### TBD: Check if maven-compiler-plugin works well with Java 10.

```xml
...
    <build>

        <plugins> 
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-compiler-plugin</artifactId>
                <version>3.7.0</version>
                <configuration>
                    <release>10</release>
                </configuration>
                <dependencies>
                    <dependency>
                        <groupId>org.ow2.asm</groupId>
                        <artifactId>asm</artifactId>
                        <version>6.1.1</version> <!-- use newer version of ASM -->
                    </dependency>
                </dependencies>
            </plugin>
        </plugins>

    <build>
...
```
