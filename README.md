# zn-docker
This is docker note for zeronote.

## LXC
LXC 是Linux Container的英文缩写，代表了Linux容器技术。Docker是目前最流行的容器技术。
和LXC相对的有VPC技术，那么既然又了VPC技术，我们为什么还选择LXC技术呢。我们来看看LXC技术的优势：

## LXC技术优势
* 秒级／微秒级部署
LXC的部署速度非常快，可以达到秒级甚至微秒级的部署速度。
* 近似于裸机的运行性能
LXC不需要额外Hypervisor技术支持,他是内核级的虚拟化
* 虚拟机般的便捷－－并且仍然是“虚拟化”技术
LXC虽然不同于VPC，但是他仍然是虚拟化技术之一，有着虚拟化技术的各种特性和优势，却没有VPC的庞大。
* 轻量级
运行某个应用的容器，更加像是这个应用本身，基本不消耗任何额外资源。运行容器的物理机，系统资源利用率非常高，一台服务器上可以运行数百甚至数千个容器甚至更多。
* 高可移植性
LXC几乎可以在任意平台运行，虚拟机、物理机、共有云、私有云

Docker
* 商品化的开源容器引擎
* 写时拷贝（Copy on Write）
* 允许制作及共享镜像

Docker对于传统LXC有哪些新东西
* 多主机间的可移植部署
* 专注于应用
* 自动化构建
* 版本控制
* 镜像重用及共享
* 工具集－CLI/REST API

## 容器集群管理
### 容器集群管理要解决的问题
* 面向服务的体系结构（SOA）/微服务体系结构
* 多种持久化混合方案
* 健全的容错机制／高可用性
* 可扩展性
* 高效性
### 典型的容器管理工具有以下几类
* 容器调度（例如：Docker Swarm、Kubernetes、Apache Mesos、CoreOS Fleet、Openstack Magnum）
* 配置管理（Etcd、Zookeeper、Consul）
* 服务发现（Etcd、Haproxy、Consul）
* 日志／监控／报警（ELK stack、cAdvisor、Prometheus）

## CaaS概述
云集规模容器管理系统，要解决如下的问题：
* 容器调度
* 服务发现
* 网络配置
* 安全配置
* 负载均衡
* 数据持久化
* 容错／高可用
* 日志管理／容器监控

CaaS的出现打破传统云计算三层结构，提供了Docker管理的全面方案：
* 提供了容器的运行平台并管理容器所需的资源
* IaaS般的灵活，PaaS般的便利
* 支持多租户
* 伸缩性－弹性的扩大和缩小所需要的资源
* 可视化（UI）和可控性


CaaS概述－CaaS的机遇和挑战
机遇
* 共享了容器技术所带来的所有优势
* 解决了laaS和PaaS在实践中存在的问题
* 使应用开发者专注于应用开发
* 快速迭代，简化部署
* 微服务的理想平台
挑战
* 共享容器技术的不足
* 前沿技术，日新月异
* 容器镜像云平台化
* 国内社区不够成熟，认知度低

CaaS服务平台
目前比较大的CaaS服务平台厂商有：  
国内：灵雀云  
国外：amazon、google、microsoft azure、rancher、tutum  


## Relevant Helps
#### <a href="http://www.appinn.com/markdown/">Markdown 语法说明 (简体中文版)</a>

