# scm-master-pom
## Master pom for Maven projects

Usage:
```
    <project xmlns="http://maven.apache.org/POM/4.0.0" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">

        <modelVersion>4.0.0</modelVersion>

        <parent>
            <groupId>com.leonardocantoni.scm</groupId>
            <artifactId>scm-master-pom</artifactId>
            <version>x.x.x</version>
        </parent>

        <groupId>my-group</groupId>
        <artifactId>my-artifact</artifactId>
        <version>x.x.x</version>

        ...

    </project>
```

This master pom pre-configures the following maven plugins:

 + Maven deploy plugin
 + Maven release plugin
 + Maven compiler plugin, configured for java 8 by default.
 + Maven javadoc plugin, skipped by default. For activate, add the following property:
 
 ```
 <maven-javadoc-plugin.skip>false</maven-javadoc-plugin.skip>
 ```
 + Versions maven plugin. Output file: ${basedir}/target/versions-maven-plugin-result.txt
 + Dependency check maven plugin, skipped by default. For activate, add the following property:
 
 ```
 <dependency-check-maven.skip>false</dependency-check-maven.skip>
 ```

Badge | Status
--- | ---
**License** |  [![Apache license](https://img.shields.io/github/license/leonardocantoni/scm-master-pom.svg)](https://www.apache.org/licenses/LICENSE-2.0)
**Travis CI Build** | [![Build Status](https://travis-ci.org/leonardocantoni/scm-master-pom.svg?branch=master)](https://travis-ci.org/leonardocantoni/scm-master-pom)
**Issue Count** | [![Issue Count](https://lima.codeclimate.com/github/leonardocantoni/scm-master-pom/badges/issue_count.svg)](https://lima.codeclimate.com/github/leonardocantoni/scm-master-pom)
**Version Eye** | [![Version Eye Dependency Status](https://www.versioneye.com/user/projects/58c1648ac920cf0032e3d9ed/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/58c1648ac920cf0032e3d9ed#tab-dependencies)
**Latest Release Version** | [![Current Version](https://img.shields.io/github/release/leonardocantoni/scm-master-pom.svg)](https://github.com/leonardocantoni/scm-master-pom/releases/latest)

