# Kubernetes技术实践（进阶篇）

大家好，很快又和大家见面了，在前面的Kubernetes技术实践--基础篇中，我给你讲了如何将微服务部署到Kubernetes测试集群中，让你对Kubernetes的使用有了一个初步的认识。在基础篇中我并没有给你展开来讲Kubernetes的一些技术细节，在接下来的进阶篇中让我们一起深入了解Kubernetes。

为了实现大家对Kubernetes系统化学习及对周边生态掌握，经半年多的筹备，我们特别推出了这个实战课程，课程内容规划原则：系统化、实战化、生产可用化，让所有学员能系统化深入学习Kubernetes以及容器相关技术，少走弯路。

为了让大家有更真实的体验，在这个培训课程中，我虚拟了一家互联网创业公司，而我们就是这家创业公司的技术人员，我们要从0开始为这家创业公司搭建IT环境，我们的所有服务都是容器化的，并运行在Kubernetes高可用集群上。我们的产品是由十一个微服务组成时尚购物网站，这十一个微服务由不同的语言写成，包括Java、Go、Python、Node.js和C#。我们通过CI/CD流水线驱动这些服务的开发迭代，并通过Istio进行服务治理，我们可以通过蓝绿部署、金丝雀部署、服务限流、熔断、链路追踪等技术来提升客户体验。我们为这家虚拟公司购买了域名（hipstershop.cn）和SSL证书，并完成了备案-_^，接下来，我们将一起完成这家公司的IT环境搭建。

## 能学到什么？

- **搭建生产环境可用的Kubernetes集群** 我会从Kubernetes的架构开始讲起，然后给大家介绍Kubernetes的主要组件以及一些基本概念，接下带大家一起部署生产环境可用的Kubernetes集群，安装Kubernetes常用的插件，接下来为大家讲解在生成环境如何去升级已有的Kubernetes集群，最后为大家介绍如何轻松管理多个Kubernetes集群；
- **部署企业级私有仓库** 这部分我会带领大家讲一起部署企业级代码管理平台Gitlab和容器私有仓库Harbor，学完这部分内容你将掌握如何通过容器化的方式部署Gitlab和Harbor，以及Gitlab和Harbor的基本使用；
- **Kubernetes编排基础** 这部分我会详细向你讲解Pod基础与进阶，包括Pod的生命周期管理、升级回滚、扩缩容、健康检查及生产环境建议及操作实践；Kubernetes常用资源对象操作，主要包括ReplicaSet、Deployment、StatefulSet、DeamonSet、Job等等；权限控制，包括ServiceAccount介绍、RBAC基于角色的访问控制、NetworkPolicy等等；
- **Kubernetes网络选型** 这部分我会向你讲解容器跨主机网络、Kubernetes网络模型与CNI网络插件、常用的三层网络方案、以及Kubernetes服务发现，包括集群内部服务发现(Servcie)、集群外部服务访问(Ingress)、Headkess服务、CoreDNS以及4/7层服务发现实践；
- **Kubernetes容器持久化存储** 这部分我会向你讲解容器卷、PV、PVC、StorageClass以及本地化持久存储相关的知识，最后会带你实践如何使用Ceph分布式存储和阿里云云盘作为Kubernetes容器持久化存储；
- **Kubernetes包管理工具Helm** 这部分我会向你讲解如何搭建私有Helm仓库、如何使Helm使用仓库、如何编写Helm Charts，并带领你为我们的微服务编写charts，并上传等到私有Helm仓库；
- **CI/CD流水线** 这部分我会向你讲解CI/CD流水线技术，并带你认识几种CI/CD产品，介绍他们如何配置、使用，然后带你使用CI/CD流水线将微服务部署到Kubernetes集群上，通过使用CI/CD流水线来提升我们的开发、测试、部署流程的自动化水平；
- **Kubernetes日志管理** 这部分我会向你讲解Kubernetes日志处理的基本原理，以及如何通过EFK收集Kubernetes集群的日志及微服务产生的日志；
- **Kubernetes监控** 这部分我会向你讲解Kubernetes监控原理，如何部署Prometheus，并使用其进行集群及应用监控，结合AlertManager实现故障告警；
- **通过Istio实现服务治理** 这部分我会向你讲解Istio是什么，他能做什么，以及如何使用Istio实现微服务服务的蓝绿部署、金丝雀部署，如何对服务进行限流、熔断和链路追踪。

## 学员收获

- 从0-1全系统化学习Kubernetes，对调度系统、网络、存储、日志监控、CI/CD、服务治理等有全局了解，熟悉学习路线；
- 提高Kubernetes技术在企业落地效率，生产实践路上少走弯路；
- 熟悉Kubernetes生产最佳实践，避免踩坑；
- 专属QQ交流群，有任何问题老师会在群里给大家答疑
- 代码开发，课程案例代码完全开发给你，你可以根据所学知识自行修改、优化

## 适合人群

- 容器基础薄弱，但对容器生态技术有浓厚兴趣的小伙伴
- 已经将容器用于生产环境，但是希望获得最佳实践，避免少走弯路的小伙伴
- 对容器技术有一定了解和接触，期望系统化的深入理解的小伙伴
- 容器技术爱好者、云计算从业者、运维工程师、容器项目开发工程师、架构师

## 技术储备要求

- 熟悉基本Linux操作
- 熟悉Docker容器概念与原来，如果对容器基础概念不熟悉建议先学习：https://github.com/findsec-cn/docker课程
- 熟悉yaml语法，建议学习：http://www.ruanyifeng.com/blog/2016/07/yaml.html
