OSGi source bundles
===================

Maven projects to generate source bundles for some JSON libraries.

It generates the bundles for the following projects:
 - com.fasterxml.jackson.core:jackson-core
 - com.fasterxml.jackson.core:jackson-annotations
 - com.fasterxml.jackson.core:jackson-databind
 - javax.json:javax.json-api
 - com.fasterxml.jackson.datatype:jackson-datatype-jsr353
 - com.fasterxml.jackson.dataformat:jackson-dataformat-xml
 - com.github.fge:jackson-coreutils
 - com.github.fge:msg-simple
 - com.github.fge:btf
 - org.codehaus.woodstox:woodstox-core-asl
 - org.codehaus.woodstox:stax2-api
 - com.fasterxml.jackson.module:jackson-module-jaxb-annotations
 - net.minidev:asm
 - com.github.fge:json-path
 - net.sf.jopt-simple:jopt-simple
 - com.github.fge:json-schema-core
 - com.github.fge:json-schema-validator
 - com.github.fge:uri-template
 - joda-time:joda-time
 - com.github.fge:json-patch

[![Build Status](https://travis-ci.org/aborg0/osgi_source_bundles.svg?branch=master)](https://travis-ci.org/aborg0/osgi_source_bundles)

Usage
-----

`mvn package` or `mvn install` (with the latter you can use the `~/.m2/repository.xml` to add to the target platform)

Copy the generated source bundles to your target platform with a command like the following:

    find . -name "*.jar" -exec cp '{}' /path/to/my/targetPlatform/ \;
