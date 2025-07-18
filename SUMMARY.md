# Table of contents

* [序言](README.md)

## 基础入门 <a id="introduction"></a>

* [Kubernetes 简介](introduction/index.md)
* [Kubernetes 基本概念](introduction/concepts.md)
* [Kubernetes 101](introduction/101.md)
* [Kubernetes 201](introduction/201.md)
* [Kubernetes 集群](introduction/cluster.md)

## 核心原理 <a id="concepts"></a>

* [核心原理](concepts/index.md)
* [架构原理](concepts/architecture.md)
* [设计理念](concepts/concepts.md)
* [核心组件](concepts/components/README.md)
  * [etcd](concepts/components/etcd.md)
  * [kube-apiserver](concepts/components/apiserver.md)
  * [kube-scheduler](concepts/components/scheduler.md)
  * [kube-controller-manager](concepts/components/controller-manager.md)
  * [kubelet](concepts/components/kubelet.md)
  * [kube-proxy](concepts/components/kube-proxy.md)
  * [kube-dns](concepts/components/kube-dns.md)
  * [Federation](concepts/components/federation.md)
  * [kubeadm](concepts/components/kubeadm.md)
  * [hyperkube](concepts/components/hyperkube.md)
  * [kubectl](concepts/components/kubectl.md)
* [资源对象](concepts/objects/README.md)
  * [Autoscaling](concepts/objects/autoscaling.md)
  * [ConfigMap](concepts/objects/configmap.md)
  * [CronJob](concepts/objects/cronjob.md)
  * [CustomResourceDefinition](concepts/objects/customresourcedefinition.md)
  * [DaemonSet](concepts/objects/daemonset.md)
  * [Deployment](concepts/objects/deployment.md)
  * [Gateway API](concepts/objects/gateway-api.md)
  * [Ingress](concepts/objects/ingress.md)
  * [Job](concepts/objects/job.md)
  * [LocalVolume](concepts/objects/local-volume.md)
  * [Namespace](concepts/objects/namespace.md)
  * [NetworkPolicy](concepts/objects/network-policy.md)
  * [Node](concepts/objects/node.md)
  * [PersistentVolume](concepts/objects/persistent-volume.md)
  * [Pod](concepts/objects/pod.md)
  * [PodPreset](concepts/objects/podpreset.md)
  * [ReplicaSet](concepts/objects/replicaset.md)
  * [Resource Quota](concepts/objects/quota.md)
  * [Secret](concepts/objects/secret.md)
  * [SecurityContext](concepts/objects/security-context.md)
  * [Service](concepts/objects/service.md)
  * [ServiceAccount](concepts/objects/serviceaccount.md)
  * [StatefulSet](concepts/objects/statefulset.md)
  * [Volume](concepts/objects/volume.md)

## 部署配置 <a id="setup"></a>

* [部署指南](setup/index.md)
* [kubectl 安装](setup/kubectl.md)
* [单机部署](setup/single.md)
* [特性开关](setup/feature-gates.md)
* [最佳配置](setup/kubernetes-configuration-best-practice.md)
* [版本支持](setup/upgrade.md)
* [集群部署](setup/cluster/README.md)
  * [kubeadm](setup/cluster/kubeadm.md)
  * [kops](setup/cluster/kops.md)
  * [Kubespray](setup/cluster/kubespray.md)
  * [Azure](setup/cluster/azure.md)
  * [Windows](setup/cluster/windows.md)
  * [LinuxKit](setup/cluster/k8s-linuxkit.md)
  * [kubeasz](https://github.com/gjmzj/kubeasz)
* [附加组件](setup/addon-list/README.md)
  * [Addon-manager](setup/addon-list/addon-manager.md)
  * [DNS](setup/addon-list/kube-dns.md)
  * [Dashboard](setup/addon-list/dashboard.md)
  * [监控](setup/addon-list/monitor.md)
  * [日志](setup/addon-list/logging.md)
  * [Metrics](setup/addon-list/metrics.md)
  * [GPU](setup/addon-list/gpu.md)
  * [Cluster Autoscaler](setup/addon-list/cluster-autoscaler.md)
  * [ip-masq-agent](setup/addon-list/ip-masq-agent.md)
* [Kubernetes-The-Hard-Way](setup/k8s-hard-way/README.md)
  * [准备部署环境](setup/k8s-hard-way/01-prerequisites.md)
  * [安装必要工具](setup/k8s-hard-way/02-client-tools.md)
  * [创建计算资源](setup/k8s-hard-way/03-compute-resources.md)
  * [配置创建证书](setup/k8s-hard-way/04-certificate-authority.md)
  * [配置生成配置](setup/k8s-hard-way/05-kubernetes-configuration-files.md)
  * [配置生成密钥](setup/k8s-hard-way/06-data-encryption-keys.md)
  * [部署 Etcd 群集](setup/k8s-hard-way/07-bootstrapping-etcd.md)
  * [部署控制节点](setup/k8s-hard-way/08-bootstrapping-kubernetes-controllers.md)
  * [部署计算节点](setup/k8s-hard-way/09-bootstrapping-kubernetes-workers.md)
  * [配置 Kubectl](setup/k8s-hard-way/10-configuring-kubectl.md)
  * [配置网络路由](setup/k8s-hard-way/11-pod-network-routes.md)
  * [部署 DNS 扩展](setup/k8s-hard-way/12-dns-addon.md)
  * [烟雾测试](setup/k8s-hard-way/13-smoke-test.md)
  * [删除集群](setup/k8s-hard-way/14-cleanup.md)

## 插件扩展 <a id="extension"></a>

* [API 扩展](extension/api/README.md)
  * [Aggregation](extension/api/aggregation.md)
  * [CustomResourceDefinition](extension/api/customresourcedefinition.md)
* [访问控制](extension/auth/README.md)
  * [认证](extension/auth/authentication.md)
  * [RBAC 授权](extension/auth/rbac.md)
  * [准入控制](extension/auth/admission.md)
* [Scheduler 扩展](extension/scheduler.md)
* [网络插件](extension/network/README.md)
  * [CNI](extension/network/cni.md)
  * [Flannel](extension/network/flannel.md)
  * [Calico](extension/network/calico.md)
  * [Weave](extension/network/weave.md)
  * [Cilium](extension/network/cilium.md)
  * [OVN](extension/network/ovn-kubernetes.md)
  * [Contiv](extension/network/contiv.md)
  * [SR-IOV](extension/network/sriov.md)
  * [Romana](extension/network/romana.md)
  * [OpenContrail](extension/network/opencontrail.md)
  * [Kuryr](extension/network/kuryr.md)
* [运行时插件 CRI](extension/cri/README.md)
  * [CRI-tools](extension/cri/cri-tools.md)
  * [Frakti](extension/cri/frakti.md)
* [存储插件](extension/volume/README.md)
  * [容器存储接口 CSI](extension/volume/csi.md)
  * [FlexVolume](extension/volume/flex-volume.md)
  * [glusterfs](extension/volume/glusterfs.md)
* [网络策略](extension/network-policy.md)
* [Ingress Controller](extension/ingress/README.md)
  * [Ingress + Letsencrypt](extension/ingress/ingress_letsencrypt.md)
  * [minikube Ingress](extension/ingress/minikube-ingress.md)
  * [Traefik Ingress](extension/ingress/service-discovery-and-load-balancing.md)
  * [Keepalived-VIP](extension/ingress/keepalived-vip.md)
* [Cloud Provider 扩展](extension/cloud-provider.md)
* [Device 插件](extension/device.md)

## 服务治理 <a id="apps"></a>

* [服务治理](apps/index/README.md)
  * [一般准则](apps/index/patterns.md)
  * [滚动升级](apps/index/service-rolling-update.md)
  * [Helm](apps/index/helm.md)
  * [Operator](apps/index/operator.md)
  * [Service Mesh](apps/index/service-mesh.md)
  * [Linkerd](apps/index/linkerd.md)
  * [Linkerd2](apps/index/linkerd2.md)
* [Istio](apps/istio/README.md)
  * [安装](apps/istio/istio-deploy.md)
  * [流量管理](apps/istio/istio-traffic-management.md)
  * [安全管理](apps/istio/istio-security.md)
  * [策略管理](apps/istio/istio-policy.md)
  * [度量管理](apps/istio/istio-metrics.md)
  * [排错](apps/istio/istio-troubleshoot.md)
  * [社区](apps/istio/istio-community.md)
* [Devops](apps/devops/README.md)
  * [Draft](apps/devops/draft.md)
  * [Jenkins X](apps/devops/jenkinsx.md)
  * [Spinnaker](apps/devops/spinnaker.md)
  * [Kompose](apps/devops/kompose.md)
  * [Skaffold](apps/devops/skaffold.md)
  * [Argo](apps/devops/argo.md)
  * [Flux GitOps](apps/devops/flux.md)

## 实践案例 <a id="practice"></a>

* [实践概览](practice/index.md)
* [资源控制](practice/resource-management.md)
* [集群高可用](practice/ha.md)
* [应用高可用](practice/app-ha.md)
* [调试](practice/debugging.md)
* [端口映射](practice/portmap.md)
* [端口转发](practice/portforward.md)
* [用户管理](practice/user-management.md)
* [GPU](practice/gpu.md)
* [HugePage](practice/hugepage.md)
* [安全](practice/security.md)
* [审计](practice/audit.md)
* [备份恢复](practice/backup.md)
* [证书轮换](practice/certificate-rotation.md)
* [大规模集群](practice/big-cluster.md)
* [大数据与机器学习](practice/introduction/README.md)
  * [Spark](practice/introduction/spark.md)
  * [Tensorflow](practice/introduction/tensorflow.md)
* [Serverless](practice/serverless.md)

## 排错指南 <a id="troubleshooting"></a>

* [排错概览](troubleshooting/index.md)
* [集群排错](troubleshooting/cluster.md)
* [Pod 排错](troubleshooting/pod.md)
* [网络排错](troubleshooting/network.md)
* [PV 排错](troubleshooting/pv/README.md)
  * [AzureDisk](troubleshooting/pv/azuredisk.md)
  * [AzureFile](troubleshooting/pv/azurefile.md)
* [Windows 排错](troubleshooting/windows.md)
* [云平台排错](troubleshooting/cloud/README.md)
  * [Azure](troubleshooting/cloud/azure.md)
* [排错工具](troubleshooting/tools.md)

## 社区贡献 <a id="community"></a>

* [开发指南](community/index.md)
* [单元测试和集成测试](community/testing.md)
* [社区贡献](community/contribute.md)

## 附录 <a id="appendix"></a>

* [生态圈](appendix/ecosystem.md)
* [学习资源](appendix/tutorial.md)
* [国内镜像](appendix/mirrors.md)
* [如何贡献](appendix/contributing.md)
* [参考文档](appendix/reference.md)

