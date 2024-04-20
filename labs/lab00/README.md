# Lab 00 - Setup

Confirm access in your lab environment and in your AWS account. Start minikube locally and verify.

Walk through https://docs.aws.amazon.com/eks/latest/userguide/getting-started.html, https://docs.aws.amazon.com/eks/latest/userguide/metrics-server.html, and https://docs.aws.amazon.com/eks/latest/userguide/getting-started-console.html#eks-configure-kubectl to configure EKS cluster.

Use https://repost.aws/knowledge-center/eks-persistent-storage to enable Persistent Storage in the EKS cluster.

When complete, you should have 2 clusters - minikube (local) and an EKS cluster.

NOTES - When installing in ACG:
* Follow along with the instructions in the previous links
* To enable PV creation in the ACG EKS cluster, find the NodeInstanceRole associated to the cluster and add "AmazonEC2FullAccess" to it
* Use this environment to demo labs 3, 4, and 5
* Update "Advanced K8S" environment with svc URLs from `kubectl get svc`; make sure "Advanced K8S" environment is selected with the toyshop POSTMan collection
