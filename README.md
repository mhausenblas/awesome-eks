![EKS logo](images/eks-logo.png)

A curated list of awesome tools for Amazon EKS 🌊

Want to add something? Open a PR! 🙂

## What is EKS
Amazon Elastic Kubernetes Service (Amazon EKS) is a managed service that makes it easy for you to run Kubernetes on AWS without needing to stand up or maintain your own Kubernetes control plane. Kubernetes is an open-source system for automating the deployment, scaling, and management of containerized applications.

Amazon EKS runs Kubernetes control plane instances across multiple Availability Zone to ensure high availability. Amazon EKS automatically detects and replaces unhealthy control plane instances, and it provides automated version upgrades and patching for them.

Amazon EKS runs up-to-date versions of the open-source Kubernetes software, so you can use all the existing plugins and tooling from the Kubernetes community. Applications running on Amazon EKS are fully compatible with applications running on any standard Kubernetes environment, whether running in on-premises data centers or public clouds. This means that you can easily migrate any standard Kubernetes application to Amazon EKS without any code modification required.


## Table of content
- [Cluster management tools](#cluster-management-tools)
- [Data plane management](#data-plane-management)
- [CLI tools](#cli-tools)
- [Package managers](#package-managers)
- [Security](#security)
- [Networking](#networking)
- [Compliance](#compliance)
- [Container runtime security](#container-runtime-security)
- [Audit](#audit)
- [Monitoring](#monitoring)
- [Logging](#logging)
- [Tracing](#tracing)
- [CI and CD tools](#ci-and-cd-tools)
- [Scaling](#pod-scaling)
- [Chaos testing](#chaos-testing)
- [Storage](#storage)
- [Ingress](#ingress)
- [API gateways](#api-gateways)
- [Service meshes](#service-meshes)
- [Backup](#backup)
- [Cost allocation](#cost-allocation)
- [Machine learning](#machine-learning)
- [Self-paced learning](#self-paced-learning)
- [Miscellaneous](#miscellaneous)
- [re:Invent 2019 sessions](#re-invent-2019-sessions)
- [Twitter](#twitter)
- [Books](#books)
- [Contributors](#contributors)

---


## Cluster management tools

* [eksctl](https://eksctl.io)
* [AWS CloudFormation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-eks-cluster.html)
* [cdk8s](https://github.com/awslabs/cdk8s) - Define Kubernetes native apps and abstractions using object-oriented programming
* [CDK Amazon EKS Construct Library](https://docs.aws.amazon.com/cdk/api/latest/docs/aws-eks-readme.html)
* [Terraform](https://www.terraform.io/docs/providers/aws/guides/eks-getting-started.html)
* [Pulumi](https://www.pulumi.com/docs/tutorials/kubernetes/eks/)
* [Octant](https://github.com/metral/octumi) - Deploy VMware Octant on a EKS Cluster using Pulumi
* [ekstender](https://github.com/mreferre/ekstender) - tool that extends a vanilla Amazon EKS cluster with a number of add-on OSS projects.


## Data plane management
* [Managed nodes groups](https://docs.aws.amazon.com/eks/latest/userguide/managed-node-groups.html)
* [AWS Node Termination Handler](https://github.com/aws/aws-node-termination-handler)

## CLI tools
* [Krew](https://krew.sigs.k8s.io) - a plugin manager for kubectl
* [kubectl-plugins](https://github.com/jordanwilson230/kubectl-plugins)
* [kubectx](https://github.com/ahmetb/kubectx) — Faster way to switch between clusters and namespaces in kubectl 
* [kui](https://github.com/IBM/kui/) - A hybrid command-line/UI development experience for cloud-native development
* [kubectl debug](https://github.com/aylei/kubectl-debug) - Debug your pod by a new container with every troubleshooting tools pre-installed
* [k9s](https://github.com/derailed/k9s) - Provides a terminal UI to interact with your Kubernetes clusters
* [kubectl tree](https://github.com/ahmetb/kubectl-tree)

## Package managers
* [Helm](https://docs.aws.amazon.com/eks/latest/userguide/helm.html) - The Kubernetes Package Manager
* [Amazon EKS Helm chart repository](https://github.com/aws/eks-charts)

## Security
* [Using EKS encryption provider support for defense-in-depth](https://aws.amazon.com/blogs/containers/using-eks-encryption-provider-support-for-defense-in-depth/)
* [Gatekeeper](https://github.com/open-policy-agent/gatekeeper)
* [Open Policy Agent](https://aws.amazon.com/blogs/opensource/using-open-policy-agent-on-amazon-eks/)
* [Bane](https://github.com/genuinetools/bane) - Custom & better AppArmor profile generator for Docker containers.
* [IAM Roles for service accounts](https://docs.aws.amazon.com/eks/latest/userguide/iam-roles-for-service-accounts.html)
* [eksuser](https://github.com/prabhatsharma/eksuser/) - Utility to manage Amazon EKS users
* [Sysdig Falco](hhttps://sysdig.com/blog/amazon-eks-monitoring-and-security-with-sysdig/)
* [cert-manager](https://aws.amazon.com/blogs/containers/securing-eks-ingress-contour-lets-encrypt-gitops/)
* [Pod security policy](https://docs.aws.amazon.com/eks/latest/userguide/pod-security-policy.html)
* [kube-hunter](https://github.com/aquasecurity/kube-hunter)

## Networking
* [AWS VPC CNI](https://github.com/aws/amazon-vpc-cni-k8s)
* [CNI metrics helper](https://docs.aws.amazon.com/eks/latest/userguide/cni-metrics-helper.html)
* [Calico network policy engine for Kubernetes](https://docs.aws.amazon.com/eks/latest/userguide/calico.html)
* [Cluster VPC considerations](https://docs.aws.amazon.com/eks/latest/userguide/network_reqs.html)
* [ksniff](https://github.com/eldadru/ksniff) - Kubectl plugin to ease sniffing on kubernetes pods using tcpdump and wireshark


## Compliance
* [kube-bench](https://github.com/aquasecurity/kube-bench#running-in-an-eks-cluster)
* [docker-bench-security](https://github.com/docker/docker-bench-security)
* [actuary](https://github.com/diogomonica/actuary)
* [AWS Inspector](https://aws.amazon.com/inspector/)
* [Sysdig Secure](https://sysdig.com/products/kubernetes-security/)

## Container runtime security
* [Aqua](https://www.aquasec.com/products/aqua-cloud-native-security-platform/)
* [Qualys](https://www.qualys.com/apps/container-security/)
* [Amazon ECR container image scanning](https://docs.aws.amazon.com/AmazonECR/latest/userguide/image-scanning.html)
* [Twistlock](https://www.twistlock.com/2017/11/29/elastic-container-service-kubernetes-amazon-eks-twistlock/)

## Audit
* [Logging Amazon EKS API calls with AWS CloudTrail](https://docs.aws.amazon.com/eks/latest/userguide/logging-using-cloudtrail.html)
* [kubeaudit](https://github.com/Shopify/kubeaudit)
* [MKIT](https://github.com/darkbitio/mkit#example-run-against-an-eks-cluster)
* [kubesec.io](https://kubesec.io/)
* [polaris](https://aws.amazon.com/blogs/opensource/running-secure-workloads-eks-polaris/)

## Monitoring
* [Kubernetes Metrics Server](https://docs.aws.amazon.com/eks/latest/userguide/metrics-server.html) — Cluster-wide aggregator of resource usage data
* [kube-state-metrics](https://github.com/kubernetes/kube-state-metrics) — Add-on agent to generate and expose cluster-level metrics.
* [Prometheus + Grafana](https://eksworkshop.com/intermediate/240_monitoring/)
* [CloudWatch Container Insights](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/ContainerInsights.html)
* [Using Prometheus Metrics in Amazon CloudWatch](https://aws.amazon.com/blogs/containers/using-prometheus-metrics-in-amazon-cloudwatch/)

## Troubleshooting
* [kubespy](https://github.com/pulumi/kubespy)
* [Sloop](https://github.com/salesforce/sloop)

## Logging
* [Amazon EKS control plane logging](https://docs.aws.amazon.com/eks/latest/userguide/control-plane-logs.html)
* [Fluentd](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Container-Insights-setup-logs.html) — Set Up FluentD as a DaemonSet to Send Logs to CloudWatch Logs
* [Kubernetes Logging powered by AWS for Fluent Bit](https://aws.amazon.com/blogs/containers/kubernetes-logging-powered-by-aws-for-fluent-bit/)
* [Cloudwatch Container Insights](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Container-Insights-setup-EKS-quickstart.html)

## Tracing
* [AWS X-Ray](https://aws.amazon.com/xray/)
* [Jaeger](https://github.com/jaegertracing/jaeger)

## CI & CD tools
* [Flux](https://github.com/fluxcd/flux) - The GitOps Kubernetes operator
* [Flagger](https://docs.flagger.app/install/flagger-install-on-eks-appmesh) - Progressive Delivery Operator for Kubernetes
* [Spinnaker](https://github.com/spinnaker/spinnaker)
* Jenkins
* Travis
* [Circle CI](https://circleci.com/integrations/kubernetes/)
* [Gitlab](https://docs.gitlab.com/ee/user/project/clusters/add_eks_clusters.html)
* [Shippable](http://docs.shippable.com/getting-started/tutorials/)
* [Argo](https://eksworkshop.com/advanced/410_batch/deploy/)

## Pod Scaling
* [Goldilocks vertical-pod-autoscaler](https://github.com/FairwindsOps/goldilocks/)
* [kube-metrics-adapter](https://github.com/zalando-incubator/kube-metrics-adapter)
* [right-size-guide](https://github.com/mhausenblas/right-size-guide) — A CLI tool providing memory & CPU recommendations for containerized apps

## Chaos testing
* [Gremlin](https://www.gremlin.com/community/tutorials/how-to-install-and-use-gremlin-with-eks/)
* [Chaos Mesh](https://github.com/pingcap/chaos-mesh)
* [PowerfulSeal](https://github.com/bloomberg/powerfulseal)
* [kube-monkey](https://github.com/asobti/kube-monkey)
* [chaoskube](https://github.com/linki/chaoskube)

## Storage
* [Amazon EBS CSI driver](https://github.com/kubernetes-sigs/aws-ebs-csi-driver)
* [Amazon EFS CSI driver](https://github.com/kubernetes-sigs/aws-efs-csi-driver)
* [Amazon FSx for Lustre CSI driver](https://github.com/kubernetes-sigs/aws-fsx-csi-driver)
* [Rook](https://github.com/rook/rook)

## Ingress 
* [ALB Ingress Controller](https://github.com/kubernetes-sigs/aws-alb-ingress-controller) - AWS ALB Ingress Controller for Kubernetes
* [Gloo](https://github.com/solo-io/gloo) - The Feature-rich, Kubernetes-native, Next-Generation API Gateway Built on Envoy
* [Traefik](https://containo.us/traefik/) — Cloud Native Edge Router
* [Nginx](https://aws.amazon.com/blogs/opensource/network-load-balancer-nginx-ingress-controller-eks/)
* [Contour](https://github.com/projectcontour/contour)

## API gateways
* [Ambassador](https://github.com/datawire/ambassador)
* [Kong](https://github.com/Kong/kong)
* [Amazon API Gateway](https://aws.amazon.com/blogs/containers/api-gateway-as-an-ingress-controller-for-eks/)

## Service meshes
* [AppMesh](https://docs.aws.amazon.com/eks/latest/userguide/appmesh-getting-started.html)
* [Istio](https://aws.amazon.com/blogs/opensource/getting-started-istio-eks/)
* [Linkderd](http://linkerd.io)
* [Consul](https://learn.hashicorp.com/consul/kubernetes/aws-k8s)

## Backup
* [Velero](https://eksworkshop.com/intermediate/280_backup-and-restore/)

## Cost allocation
* [Ocean by spot.io](https://eksworkshop.com/beginner/190_ocean/showback/)
* [kubecost](https://kubecost.com)
* [Kubernetes Opex Analytics](https://github.com/rchakode/kube-opex-analytics)


## Machine learning
* [Kubeflow](https://github.com/kubeflow/kubeflow) — Machine Learning Toolkit for Kubernetes
* [Optimizing Spark performance on Kubernetes](https://aws.amazon.com/blogs/containers/optimizing-spark-performance-on-kubernetes/)
* [__Video__ AWS re:Invent 2019: Building machine-learning infrastructure on Amazon EKS with Kubeflow (CON306-R1)](https://www.youtube.com/watch?v=ULlqukKVKBo)

## Self-paced learning
* [EKS Workshop](https://eksworkshop.com)
* [Amazon EKS and Kubernetes on EC2 Container Networking Workshop](https://awsk8snetworkshops.com/)
* [AWS Kubeflow Workshop](https://master.d2j834wqg8s4j0.amplifyapp.com/)
* [App Mesh Workshop](https://www.appmeshworkshop.com/)
* [Blue Green Deployment with Amazon EKS and K8s](https://awsdemoworkshops.s3.us-east-2.amazonaws.com/cicd-eks-alb-bg-cdk-workshop/public/en/index.html)
* [EKS/ECR/ECS Modernization](https://modernize.awsworkshop.io)
* [GitOps Helm Workshop](https://helm.workshop.flagger.dev/)
* [Introduction to GitOps on Amazon EKS with Weaveworks](https://weaveworks-gitops.awsworkshop.io/)


## Miscellaneous 
* [AWS container services roadmap](https://github.com/aws/containers-roadmap/projects/1)
* [Container content ideas for AWS](https://github.com/awslabs/container-content-ideas-for-aws/projects/1)
* [AWS containers blog](https://aws.amazon.com/blogs/containers/)
* [Nick Brandaleone's blog](www.nickaws.net)
* [Amazon EKS Kubernetes versions](https://docs.aws.amazon.com/eks/latest/userguide/kubernetes-versions.html#kubernetes-1.16)
* [Windows support](https://docs.aws.amazon.com/eks/latest/userguide/windows-support.html)
* [ARM Support](https://docs.aws.amazon.com/eks/latest/userguide/arm-support.html)
* [Amazon EKS on AWS Outposts](https://docs.aws.amazon.com/eks/latest/userguide/eks-on-outposts.html)
* [Awesome AWS Workshops](https://awesome-aws-workshops.com/#containers)


## re:Invent 2019 sessions
* [AWS re:Invent 2019: Running Kubernetes at Amazon scale using Amazon EKS (CON212-R1)](https://www.youtube.com/watch?v=M-Fh0OzliJI)
* [AWS re:Invent 2019: Running Kubernetes Applications on AWS Fargate (CON326-R1)](https://www.youtube.com/watch?v=m-3tMXmWWQw)
* [AWS re:Invent 2019: Amazon EKS under the hood (CON421-R1)](https://www.youtube.com/watch?v=7vxDWDD2YnM)
* [AWS re:Invent 2019: Building machine-learning infrastructure on Amazon EKS with Kubeflow (CON306-R1)](https://www.youtube.com/watch?v=ULlqukKVKBo)


## Twitter
* [Nathan Peck](https://twitter.com/nathankpeck) - AWS Developer Advocate
* [Massimo Re Ferre'](https://twitter.com/mreferre) - AWS Developer Advocate
* [Michael Hausenblas](https://twitter.com/mhausenblas) - AWS Developer Advocate

## Books
* Container Security by Liz Rice
* Kubernetes Patterns by Roland Huß
* Kubernetes Best Practices by Lachlan Evenson, Dave Strebel, Eddie Villalba, Brendan Burns
* Programming Kubernetes by Michael Hausenblas
* Kubernetes Cookbook by Sébastien Goasguen and Michael Hausenblas
* Mastering Kubernetes by Gigi Sayfan

## Contributors
[@realvz](https://twitter.com/realz)

