# 开放应用模型规范

开放应用模型（Open Application Model）是一份构筑云原生应用的通用规范。

_开放应用模型_ 为在诸如Kubernetes这样的平台上构建和发布应用带来了模块化、可扩展、可移植的设计，并致力于将开发者和运维人员的关注点充分分离。

*这个仓库尚未稳定，欢迎参与贡献*。
规范的内容还在编写中，依然可能出现不兼容的重大变更。
有兴趣参与贡献吗？看看[问题列表](https://github.com/oam-dev/spec/issues)吧，我们正在搜寻更多关于云原生应用模型的好主意。

## 简介

![How it works][how-it-works]

当谈到应用的开发和部署，我们认为将开发者和运营人员负责的部分加以区分十分重要。否则，如果混淆了这些角色的职责，就可能导致沟通不畅、产生BUG、甚至服务中断。

_开放应用模型_ 尝试根据构建、运行应用，以及运维基础架构的职责来划分角色。

* _开发者_ 负责描述微服务及组件的功能，以及 _如何_ 进行配置。他们是代码领域的专家。
* _应用运维人员_ 负责配置一个或多个微服务的运行时属性，他们是平台域的专家。
* _基础设施运维人员_ 负责配置和维护运行应用的基础设施。他们是底层架构领域的专家。

请阅读[introduction.md](./introduction.md)文档了解更多细节和用户故事。

## 实现案例

[Rudr](https://github.com/oam-dev/rudr)是开放应用模型基于Kubernetes的一个参考实现，通过[Rudr教程](https://github.com/oam-dev/rudr/blob/master/docs/tutorials/deploy_and_update.md)中的示例，可以立即开始体验开放应用模型。

## 规范内容

[符号约定](notational_convention.md)

  1. [目的和目标](1.purpose_and_goals.md)
  2. [概述和术语](2.overview_and_terminology.md)
  3. [组件模型](3.component_model.md)
  4. [应用边界](4.application_scopes.md)
  5. [特征](5.traits.md)
  6. [应用配置](6.application_configuration.md)
  7. [工作负载类型](7.workload_types.md)
  8. [实际问题](8.practical_considerations.md)
  9. [设计原则](9.design_principles.md)


## 社区

### 里程碑

请访问[里程碑](https://github.com/microsoft/hydra-spec/milestones)页面，获取项目里程碑的概述及详细内容。

### 任务调整 

在每两周的社区电话会议期间，会将项目任务划归到里程碑。在此会议过程中，问题可能会被纳入里程碑、从里程碑中删除，或在里程碑之间移动。

### 参与贡献

参看[贡献](CONTRIBUTING.md)文档可获得更多关于提交变更到规约的内容。

参与讨论的最简单的贡献方法之一，具体来说有以下几种渠道。

| 事项        | 信息  |
|---------------------|---|
| 邮件列表 | https://groups.google.com/forum/#!forum/oam-dev |
| 社区会议时间 | 每隔周 (从2019年10月22日开始)，周二 PST时区 早上10:30  |
| 社区会议连接 | https://zoom.us/j/271516061 |
| 即时沟通渠道 | https://gitter.im/oam-dev/ |

[how-it-works]: assets/how-it-works.png

---

中文版不定期与官方原版内容同步。当前更新至主干版本：`b32d8a9686abaecf5546256e41851aacf547a363` (2019-10-18)
