# focus-resources
Shared FocusFish resources o be used as dependency by plugins as for example code style 

### Ex for formatter-maven-plugin

```xml
  <plugin>
    <groupId>net.revelc.code.formatter</groupId>
    <artifactId>formatter-maven-plugin</artifactId>
    <version>2.7.0</version>
    <configuration>
      <configFile>eclipse-formatter-config.xml</configFile> <!-- <== uses resources from this project-->
    </configuration>
    <dependencies>
      <dependency> <!-- Include resources from this project-->
        <groupId>fish.focus.maven</groupId>
        <artifactId>focus-resources</artifactId>
        <version>[version]</version>
      </dependency>
    </dependencies>
  </plugin>
  ```
