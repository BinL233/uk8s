
# 概览


- 产品简介
  - [产品概念](/uk8s/introduction/whatisuk8s)
  - [使用须知](/uk8s/introduction/restriction)
  - [产品价格](/uk8s/price)
  - [名词解释](/uk8s/introduction/concept)
  - [使用必读](/uk8s/userguide/before_start)
  - [入门必读](/uk8s/troubleshooting/startguide)
- 集群版本
  - [维护说明](/uk8s/version/maintain)
  - 版本跟踪
    - [1.26 版本说明](/uk8s/version/1.26_release)
- 集群管理
  - [创建集群](/uk8s/userguide/createcluster)
  - [查看集群](/uk8s/userguide/describecluster)
  - [删除集群](/uk8s/userguide/deletecluster)
  - 通过 Kubectl 管理集群
    - [kubectl 命令行简介](/uk8s/manageviakubectl/intro_of_kubectl)
    - [安装及配置 kubectl](/uk8s/manageviakubectl/connectviakubectl)
    - [使用 web kubectl](/uk8s/manageviakubectl/webterminal)
    - [集群更新凭证](/uk8s/manageviakubectl/reset_token)
    - [创建 PVC](/uk8s/manageviakubectl/createpvc)
    - [创建 Service](/uk8s/manageviakubectl/createservice)
    - [StatefulSet 示例](/uk8s/manageviakubectl/sts_example)
    - [打散pod](/uk8s/manageviakubectl/pod_affinity.md)
    - [kubectl 常见问题](/uk8s/troubleshooting/kubectl)
  - [手动增加外网凭证](/uk8s/administercluster/add-external-certificate)
  - [部署Dashboard](/uk8s/administercluster/dashboard)
  - [集群版本升级](/uk8s/administercluster/cluster_version_update)
  - [集群常见问题](/uk8s/troubleshooting/cluster_summary.md)
- 节点管理
  - [集群节点配置推荐](/uk8s/introduction/node_requirements)
  - [节点池](/uk8s/administercluster/node_group)
  - [添加节点](/uk8s/userguide/addnode)
  - [虚拟节点](/uk8s/administercluster/virtual_kubelet)
  - [添加已有虚拟机节点](/uk8s/userguide/addUHostNode)
  - [添加已有裸金属节点](/uk8s/userguide/addUPHostNode)
  - [安全组支持](/uk8s/userguide/SupportSecurityGroup.md)
  - [制作自定义节点镜像](/uk8s/administercluster/custom_image)
  - [自定义节点数据及初始化脚本](/uk8s/administercluster/cloud_init)
  - [节点常见问题](/uk8s/troubleshooting/node_debug_summary)
- 集群弹性伸缩
  - [概述](/uk8s/administercluster/autoscaling/intro)
  - [弹性伸缩（HPA）](/uk8s/administercluster/autoscaling/hpa)
  - [垂直伸缩（VPA）](/uk8s/administercluster/autoscaling/vpa)
  - [定时伸缩（CronHPA）](/uk8s/administercluster/autoscaling/cronhpa)
  - [集群伸缩（CA）](/uk8s/administercluster/autoscaling/ca)
  - [基于自定义指标伸缩 Pod](/uk8s/monitor/prometheus/autoscale_on_custom_metrics.md)
- 集群网络
  - 基于 UVPC 的 underlay 网络
    - [集群网络](/uk8s/network/uk8s_network)
    - [网络隔离](/uk8s/network/networkpolicy)
    - [固定 IP 使用方法](/uk8s/network/static_ip)
    - [CNI 网络插件升级](/uk8s/network/cni_update)
    - [IPAMD](/uk8s/network/ipamd)
    - [CNI 常见问题](/uk8s/troubleshooting/cni)
- 服务发现
  - Service 管理
    - [Service 介绍](/uk8s/service/intro)
    - [集群内访问 Service](/uk8s/service/cluster_service)
    - [通过ULB 访问 Service](/uk8s/service/internalservice)
    - [使用已有的 ULB](/uk8s/service/ulb_designation)
    - [ULB 参数说明](/uk8s/service/annotations)
    - [获取真实客户端 IP](/uk8s/service/getresourceip)
    - [集群 ULB 误删处理](/uk8s/troubleshooting/ulb_undelete)
    - [ULB 常见问题](/uk8s/troubleshooting/ulb)
  - Ingress 管理
    - [概述](/uk8s/service/ingress/README)
    - [Nginx Ingress](/uk8s/service/ingress/nginx_1.19)
    - [Ingress 高级用法](/uk8s/service/ingress/multiple_ingress)
  - [CloudProvider 插件升级](/uk8s/service/cp_update)
- 集群存储
  - [Volume 介绍](/uk8s/volume/intro)
  - 块存储
    - [在 UK8S 中使用 UDISK](/uk8s/volume/udisk)
    - [在 UK8S 中使用 RSSD UDisk](/uk8s/volume/rssdudisk)
    - [UDisk 动态扩容](/uk8s/volume/expandvolume)
    - [Flexvolume 升级 CSI](/uk8s/volume/flexv_csi)
    - [RSSD 云盘挂载问题](/uk8s/troubleshooting/rssd_attachment)
    - [在节点宕机时恢复挂载了云盘的 Pod](/uk8s/troubleshooting/recover_udisk_pod_when_node_crash.md)
  - 文件存储
    - [在 UK8S 中使用 UFS](/uk8s/volume/ufs)
    - [动态PV使用UFS](/uk8s/volume/dynamic_ufs)
    - [在 UK8S 中使用 UPFS](/uk8s/volume/upfs)
  - 对象存储
    - [在 UK8S 中使用 US3](/uk8s/volume/ufile)
  - [CSI 存储插件升级](/uk8s/volume/CSI_update)
  - [存储常见问题](/uk8s/troubleshooting/storage)
- 集群监控
  - Prometheus 监控方案
    - [什么是 Prometheus](/uk8s/monitor/prometheus/intro)
    - [核心概念](/uk8s/monitor/prometheus/concept)
    - [手动部署 Prometheus](/uk8s/monitor/prometheus/installprometheus)
    - [监控中心概述](/uk8s/monitor/prometheusplugin/intro.md)
    - [监控中心开启](/uk8s/monitor/prometheusplugin/startmonitor.md)
    - [监控中心添加告警目标](/uk8s/monitor/prometheusplugin/addmonitortarget.md)
    - [监控中心添加接收人](/uk8s/monitor/prometheusplugin/addreceiver.md)
    - [监控相关常见问题](/uk8s/monitor/prometheusplugin/faq.md)
- 集群日志
  - [使用 ELK 自建 UK8S 日志解决方案](/uk8s/log/elastic_filebeat_kibana_solution)
  - [使用 UK8S 日志插件功能](/uk8s/log/ELKplugin)
  - [集群日志组件常见问题](/uk8s/troubleshooting/log_elk_summary.md)
- GPU
  - [GPU 节点](/uk8s/administercluster/gpu-node)
  - [GPU 共享插件](/uk8s/administercluster/gpu-share)
  - [GPU 监控](/uk8s/administercluster/gpu-monitor)
- 集群组件管理
  - Master 组件管理
    - [NodePort 相关参数修改](/uk8s/bestpractice/modify_nodeport)
  - Etcd
    - [ETCD 备份及恢复](/uk8s/administercluster/etcd_backup)
  - CoreDNS
    - [配置自定义 DNS 服务](/uk8s/administercluster/custom_dns_service)
  - Containerd
    - [Docker VS Containerd](/uk8s/userguide/docker_vs_containerd)
    - [Containerd 常见问题](/uk8s/troubleshooting/containerd)
  - kube-proxy
    - [kube-proxy 模式选择](/uk8s/userguide/kubeproxy_mode)
    - [kube-proxy 模式切换](/uk8s/userguide/kubeproxy_edit)
  - node-problem-detector
    - [修改 npd 配置说明](/uk8s/troubleshooting/npd.md)
  - [UK8S 核心组件故障恢复](/uk8s/administercluster/k8splugin_restore)
- 镜像仓库
  - [概述](/uk8s/dockerhub/outline)
  - [在 UK8S 中使用 UHub](/uk8s/dockerhub/using_uhub_in_uk8s)
  - [镜像及镜像仓库常见问题](/uk8s/troubleshooting/registry)
  - [推理常用基础镜像](/uk8s/dockerhub/ai_base_image_list.md)
- Kubernetes 实践
  - Pod 管理
    - [Pod 容忍节点异常时间调整](/uk8s/bestpractice/taint_base_eviction)
    - [Pod 常见故障处理](/uk8s/troubleshooting/pod_debug_summary)
  - 权限及审计
    - [RBAC 权限管理实践](/uk8s/bestpractice/rbac_practice)
    - [API Server 审计功能](/uk8s/bestpractice/apiserver_audit)
  - CI/CD 实践
    - [Docker & Jenkins](/uk8s/bestpractice/cicd)
    - [Kaniko & Jenkins](/uk8s/bestpractice/cicd_containerd)
  - [亲和性实践](/uk8s/bestpractice/affinity)
- 漏洞跟踪
  - [CVE-2019-5736](/uk8s/vulnerability/cve-2019-5736.md)
  - [CVE-2019-9512-9514](/uk8s/vulnerability/cve-2019-9512-9514.md)
  - [CVE-2021-30465](/uk8s/vulnerability/cve-2021-30465.md)
