<p align="center"><img src="./readme/new-logo.png" height="300" width="400" alt="logo"/></p>
<h2 align="center">简洁优雅 · 稳定高效 | 宁静致远 · 精益求精 </h2>

---

<p align="center">
    <a href="https://spring.io/projects/spring-boot" target="_blank"><img src="https://img.shields.io/badge/Spring%20Boot-4.1.0-blue.svg?logo=springboot" alt="Spring Boot 4.1.0"></a>
    <a href="https://spring.io/projects/spring-cloud" target="_blank"><img src="https://img.shields.io/badge/Spring%20Cloud-2025.1.1-blue.svg?logo=springboot" alt="Spring Cloud 2025.1.1"></a>
    <a href="https://github.com/alibaba/spring-cloud-alibaba" target="_blank"><img src="https://img.shields.io/badge/Spring%20Cloud%20Alibaba-2025.1.0.0-blue.svg?logo=alibabadotcom" alt="Spring Cloud Alibaba 2025.1.0.0"></a>
    <a href="https://github.com/Tencent/spring-cloud-tencent" target="_blank"><img src="https://img.shields.io/badge/Spring%20Cloud%20Tencent-2.1.2.0--2025.0.2-blue.svg?logo=qq" alt="Spring Cloud Tencent 2.1.2.0-2025.0.2"></a>
    <a href="https://nacos.io/docs/latest/overview/" target="_blank"><img src="https://img.shields.io/badge/Nacos-3.2.2-brightgreen.svg?logo=alibabadotcom" alt="Nacos 3.2.2"></a>
</p>
<p align="center">
    <a href="https://my.oschina.net/pointerv" target="_blank"><img src="https://img.shields.io/badge/Author-%E7%A0%81%E5%8C%A0%E5%90%9B-orange" alt="码匠君"></a>
    <a href="./LICENSE"><img src="https://img.shields.io/badge/License-Apache--2.0-blue.svg?logo=apache" alt="License Apache 2.0"></a>
    <a href="https://bell-sw.com/pages/downloads/#downloads" target="_blank"><img src="https://img.shields.io/badge/JDK-25%2B-green.svg?logo=openjdk" alt="Java 25"></a>
    <a href="https://github.com/dante-compass/herodotus-ecosystem-build" target="_blank"><img src="https://img.shields.io/badge/Version-4.0.7.1-red.svg?logo=spring" alt="Version 4.0.7.1"></a>
    <a href="https://github.com/dromara/dante-cloud" target="_blank"><img src="https://img.shields.io/badge/Dante%20Cloud-4.0.7.1-red.svg?logo=spring" alt="Dante Cloud 4.0.7.1"></a>
    <a href="https://github.com/dante-compass/dante-engine" target="_blank"><img src="https://img.shields.io/badge/Dante%20Engine-4.0.7.1-red.svg?logo=spring" alt="Dante Engine 4.0.7.1"></a>
    <a href="https://github.com/dante-compass/thingsbrain" target="_blank"><img src="https://img.shields.io/badge/ThingsBrain-4.0.7.1-red.svg?logo=spring" alt="ThingsBrain 4.0.7.1"></a>
    <a href="https://github.com/dante-compass/dante-cloud-ui" target="_blank"><img src="https://img.shields.io/badge/Dante%20Cloud%20UI-4.0.7.1-blue.svg?logo=quasar&logoColor=%23050A14" alt="Dante Cloud UI 4.0.7.1"></a>
    <a href="https://github.com/dante-compass/herodotus-cloud-ui-vuetify" target="_blank"><img src="https://img.shields.io/badge/Dante%20Cloud%20UI(New)-4.0.7.1-blue.svg?logo=vuetify&logoColor=%231867C0" alt="Dante Cloud UI(New) 4.0.7.1"></a>
    <a href="https://www.herodotus.cn"><img src="https://visitor-badge.laobi.icu/badge?page_id=dante-cloud&title=Total%20Visits" alt="Total Visits"></a>
</p>
<p align="center">
    <a href="https://atomgit.com/dromara/dante-cloud">Atomgit 仓库</a> &nbsp; | &nbsp;
    <a href="https://github.com/dromara/dante-cloud">Github 仓库</a> &nbsp; | &nbsp;
    <a href="https://gitee.com/dromara/dante-cloud">Gitee 仓库</a> &nbsp; | &nbsp;
    <a href="https://www.herodotus.cn">在线文档</a>
</p>

<h1 align="center"> 支持本项目除了 Fork、Pull 和 Download Zip，还可以点右上角 "Star"！</h1>

# [一]、工程介绍

`Herodotus Ecosystem Build` 为 Herodotus 软件生态 Maven 依赖版本、插件配置的统一管理工程。

通过该工程，统一管控开源版本和企业版本以及各生态产品的依赖，以保证各产品整体的体系化和一致性，降低依赖复杂度，减少因依赖引起的不必要的维护投入。

# [二]、工程结构

```shell
herodotus-ecosystem-build
├── herodotus-ecosystem-dependencies -- 软件生态依赖统一管理 Maven BOM
└── herodotus-ecosystem-parent -- 软件生态核心 Maven Parent
```

# [三]、价值意义

单独提取出 `herodotus-ecosystem-dependencies` 和 `herodotus-ecosystem-parent`，实现多工程的 Maven 依赖版本统一管理。 避免因 `dependencies` 放置在某一工程内，出现 `dependencies` 仅能以继承方式使用，引起多个工程开发编译必须顺序构建才能使用的情况。 使用 `herodotus-ecosystem-dependencies` 和 `herodotus-ecosystem-parent` 后，即使有模块依赖，各个工程也可以更独立和灵活的进行开发

- 在多模块工程中，将该工程 `dependencies` 或者 BOM 对应的 pom.xml 中，以 `herodotus-ecosystem-dependencies` 作为 Parent，可实现工程内所有的依赖的版本统一化管理，并且模块关系清晰还可以作为单独 BOM 发布。
- 在该工程的根目录下的 pom.xml 中，以 `herodotus-ecosystem-parent` 作为 Parent，可实现继承于 Spring Boot 的所有构建及依赖管理。

# [四]、关注我

<table align="center">
  <tr>
    <th align="center">
      <p>公众号：码匠君</p>
    </th>
  </tr>
  <tr>
    <td align="center">
      <img src="./readme/公众号.jpg" alt="公众号" height="200px">
    </td>
  </tr>
</table>