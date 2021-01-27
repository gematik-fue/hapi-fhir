HAPI FHIR
=========

## building fork
building fort and  publishing 
* `mvn -Dmaven.test.skip=true -P ALLMODULES,NOPARALLEL clean`
* `mvn -Dmaven.test.skip=true -P ALLMODULES,NOPARALLEL package`
* `mvn -Dmaven.test.skip=true -P ALLMODULES,NOPARALLEL install`
* `mvn -Dmaven.test.skip=true -pl hapi-fhir-server deploy`
* `mvn -Dmaven.test.skip=true -pl hapi-fhir-jpaserver-base deploy`

Configure $HOME/.m2/settings
```xml
<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0 https://maven.apache.org/xsd/settings-1.0.0.xsd">
<servers>
<server>
<id>labor-repo</id>
<username>shared_publish_user</username>
<password>***</password>
</server>
</servers>
</settings>
```


HAPI FHIR - Java API for HL7 FHIR Clients and Servers

[![Build Status](https://dev.azure.com/jamesagnew214/jamesagnew214/_apis/build/status/jamesagnew.hapi-fhir?branchName=master)](https://dev.azure.com/jamesagnew214/jamesagnew214/_build/latest?definitionId=1&branchName=master)
[![codecov](https://codecov.io/gh/jamesagnew/hapi-fhir/branch/master/graph/badge.svg)](https://codecov.io/gh/jamesagnew/hapi-fhir)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/ca.uhn.hapi.fhir/hapi-fhir-base/badge.svg)](http://search.maven.org/#search|ga|1|ca.uhn.hapi.fhir)
[![License](https://img.shields.io/badge/license-apache%202.0-60C060.svg)](https://hapifhir.io/hapi-fhir/license.html)

Complete project documentation is available here:
http://hapifhir.io

A demonstration of this project is available here:
http://hapi.fhir.org/

This project is Open Source, licensed under the Apache Software License 2.0.

Please see [this wiki page](https://github.com/jamesagnew/hapi-fhir/wiki/Getting-Help) for information on where to get help with HAPI FHIR. Please see [Smile CDR](https://smilecdr.com) for information on commercial support.
