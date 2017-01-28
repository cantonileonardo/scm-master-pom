# scm-master-pom
## Master pom for Maven projects

---

Usage:

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

---

This master pom pre-configures the following maven plugins:

 + Maven deploy plugin
 + Maven release plugin
 + Maven compiler plugin, configured for java 8 by default.
 + Maven javadoc plugin, skipped by default. For activate, add the following property:
 
    <maven-javadoc-plugin.skip>false</maven-javadoc-plugin.skip>

 + Versions maven plugin. Output file: ${basedir}/target/versions-maven-plugin-result.txt
 + Dependency check maven plugin, skipped by default. For activate, add the following property:

	<dependency-check-maven.skip>false</dependency-check-maven.skip>
