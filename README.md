# Devops : Sample Maven Application

[![License](https://img.shields.io/badge/License-Apache%202.0-brightgreen.svg)](https://opensource.org/licenses/Apache-2.0)
[![Website](https://img.shields.io/website-up-down-green-red/http/skydevops.co.in.svg?label=skydevops)]()


## Description

Sample Maven application

## Nexus - POM.xml Sample

```xml
<?xml version="1.0" encoding="UTF-8"?>

<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
  <modelVersion>4.0.0</modelVersion>

  <groupId>com.skydevops.sdtraining</groupId>
  <artifactId>sdtraining</artifactId>
  <version>1.1-SNAPSHOT</version>
  <packaging>war</packaging>

  <name>sdtraining Maven Webapp</name>
  <!-- FIXME change it to the project's website -->
  <url>http://www.example.com</url>

  <properties>
    <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
    <maven.compiler.source>1.7</maven.compiler.source>
    <maven.compiler.target>1.7</maven.compiler.target>
  </properties>

  <dependencies>
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>4.11</version>
      <scope>test</scope>
    </dependency>
  </dependencies>

  <build>
    <finalName>sdtraining</finalName>
    <pluginManagement><!-- lock down plugins versions to avoid using Maven defaults (may be moved to parent pom) -->
      <plugins>
        <plugin>
          <artifactId>maven-clean-plugin</artifactId>
          <version>3.1.0</version>
        </plugin>
        <!-- see http://maven.apache.org/ref/current/maven-core/default-bindings.html#Plugin_bindings_for_war_packaging -->
        <plugin>
          <artifactId>maven-resources-plugin</artifactId>
          <version>3.0.2</version>
        </plugin>
        <plugin>
          <artifactId>maven-compiler-plugin</artifactId>
          <version>3.8.0</version>
        </plugin>
        <plugin>
          <artifactId>maven-surefire-plugin</artifactId>
          <version>2.22.1</version>
        </plugin>
        <plugin>
          <artifactId>maven-war-plugin</artifactId>
          <version>3.2.2</version>
        </plugin>
        <plugin>
          <artifactId>maven-install-plugin</artifactId>
          <version>2.5.2</version>
        </plugin>
        <plugin>
          <artifactId>maven-deploy-plugin</artifactId>
          <version>2.8.2</version>
        </plugin>
      </plugins>
    </pluginManagement>
  </build>
  <repositories>
    <repository>
      <id>sdGroupRepo</id>
      <url>https://nexus.skydevops.in/content/repositories/thirdparty/</url>
    </repository>
  </repositories>
  <distributionManagement>
    <snapshotRepository>
      <id>sdSnapRepo</id>
      <url>https://nexus.skydevops.in/content/repositories/sdSnapRepo/</url>
    </snapshotRepository>
    <repository>
      <id>sdGroupRepo</id>
      <url>https://nexus.skydevops.in/content/repositories/thirdparty/</url>
    </repository>
  </distributionManagement>
</project>
```

## License

Licensed under the Apache License V2.0. See the [LICENSE file](LICENSE) for details.

## Author Information

You can find me on Twitter: [@skydevops](https://twitter.com/skydevops)

## Contributors

- Shashi Yebbare ([@skydevops](https://twitter.com/skydevops))