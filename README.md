# 简介

Herodotus Ecosystem Build 为 Herodotus 软件生态 Maven 依赖版本、插件配置的统一管理工程。

单独提取出 `herodotus-ecosystem-dependencies` 和 `herodotus-ecosystem-parent`，实现多工程的 Maven 依赖版本统一管理。

避免 `dependencies` 放置在某一工程内，出现 `dependencies` 仅能以继承方式使用，引起多个工程开发编译必须顺序构建才能使用的情况。

使用 `herodotus-ecosystem-dependencies` 和 `herodotus-ecosystem-parent` 后，即使有模块依赖，各个工程也可以更独立和灵活的进行开发