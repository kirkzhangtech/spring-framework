# <img src="framework-docs/src/docs/spring-framework.png" width="80" height="80"> Spring Framework [![Build Status](https://github.com/spring-projects/spring-framework/actions/workflows/build-and-deploy-snapshot.yml/badge.svg?branch=main)](https://github.com/spring-projects/spring-framework/actions/workflows/build-and-deploy-snapshot.yml?query=branch%3Amain) [![Revved up by Develocity](https://img.shields.io/badge/Revved%20up%20by-Develocity-06A0CE?logo=Gradle&labelColor=02303A)](https://ge.spring.io/scans?search.rootProjectNames=spring)

This is the home of the Spring Framework: the foundation for all [Spring projects](https://spring.io/projects). Collectively the Spring Framework and the family of Spring projects are often referred to simply as "Spring". 

Spring provides everything required beyond the Java programming language for creating enterprise applications for a wide range of scenarios and architectures. Please read the [Overview](https://docs.spring.io/spring-framework/reference/overview.html) section of the reference documentation for a more complete introduction.

## Code of Conduct

This project is governed by the [Spring Code of Conduct](https://github.com/spring-projects/spring-framework/?tab=coc-ov-file#contributor-code-of-conduct). By participating, you are expected to uphold this code of conduct. Please report unacceptable behavior to spring-code-of-conduct@spring.io.

## Access to Binaries

For access to artifacts or a distribution zip, see the [Spring Framework Artifacts](https://github.com/spring-projects/spring-framework/wiki/Spring-Framework-Artifacts) wiki page.

## Documentation

The Spring Framework maintains reference documentation ([published](https://docs.spring.io/spring-framework/reference/) and [source](framework-docs/modules/ROOT)), GitHub [wiki pages](https://github.com/spring-projects/spring-framework/wiki), and an
[API reference](https://docs.spring.io/spring-framework/docs/current/javadoc-api/). There are also [guides and tutorials](https://spring.io/guides) across Spring projects.

## Micro-Benchmarks

See the [Micro-Benchmarks](https://github.com/spring-projects/spring-framework/wiki/Micro-Benchmarks) wiki page.

## Build from Source

See the [Build from Source](https://github.com/spring-projects/spring-framework/wiki/Build-from-Source) wiki page and the [CONTRIBUTING.md](CONTRIBUTING.md) file.

## Continuous Integration Builds

Information regarding CI builds can be found in the [Spring Framework Concourse pipeline](ci/README.adoc) documentation.

## Stay in Touch

Follow [@SpringCentral](https://twitter.com/springcentral), [@SpringFramework](https://twitter.com/springframework), and its [team members](https://twitter.com/springframework/lists/team/members) on 𝕏. In-depth articles can be found at [The Spring Blog](https://spring.io/blog/), and releases are announced via our [releases feed](https://spring.io/blog/category/releases).

## License

The Spring Framework is released under version 2.0 of the [Apache License](https://www.apache.org/licenses/LICENSE-2.0).



# 项目阅读

1. spring-context是spring的核心模块，包含了IOC 和 bean factory的管理
2. GenericApplicationContext.java 和 GenericApplicationContext.java 两个重要的context的实现
3. 核心继承关系
   1. DefaultResourceLoader
      实现了基础的资源加载功能
   2. AbstractApplicationContext AbstractApplicationContext.java:140-141
      继承自 DefaultResourceLoader
      实现了 ConfigurableApplicationContext 接口
   3. GenericApplicationContext GenericApplicationContext.java:109
      继承自 AbstractApplicationContext
      实现了 BeanDefinitionRegistry 接口