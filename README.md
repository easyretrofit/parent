[![Version](https://img.shields.io/maven-central/v/io.github.easyretrofit/parent?logo=apache-maven&style=flat-square)](https://central.sonatype.com/artifact/io.github.easyretrofit/parent)
[![Build](https://github.com/easyretrofit/parent/actions/workflows/build.yml/badge.svg)](https://github.com/easyretrofit/parent/actions/workflows/build.yml/badge.svg)
[![License](https://img.shields.io/github/license/easyretrofit/parent.svg)](http://www.apache.org/licenses/LICENSE-2.0)


# easy-retrofit-parent
the parent pom of easy-retrofit, Any mainstream Java web framework extension(starter) needs to inherit this file


从3.0.0 开始, parent pom移除了如下配置, 以避免retrofit升级导致的parent文件升级
```xml
<dependencyManagement>
        <dependencies>
            <dependency>
                <groupId>com.squareup.retrofit2</groupId>
                <artifactId>retrofit</artifactId>
                <version>${retrofit.version}</version>
            </dependency>
        </dependencies>
    </dependencyManagement>
```