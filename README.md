
# Complete CI/CD with ECR & EKS

Complete CI/CD pipeline for a Java Maven application to build and push to ECR and deploy to eks cluster.






## Installation

Install Build Tool Maven in Jenkins.

Install docker, kubectl, aws-cli and “gettext-base” tool inside Jenkins.


Create Jenkins credentials for a git, ecr and AWS.

Create a eks cluster using AWS Management console or eksctl.

In Jenkins update kubeconfig file.

``` bash
aws eks update-kubeconfig --name mycluster
```

 
## Deployment

To deploy this project fork or clone this project.

Update Jenkinsfile with your ECR and git repo link.

In Jenkins create a new pipeline and add your git link.

Trigger your build.


## Screenshots

CI/CD Overview.

![Jenkins Stage View](https://gitlab.com/mujtaba.qureshi/deploy-on-k8s/-/raw/main/Images/Overview.jpg?ref_type=heads)

Jenkins Stage View.

![Jenkins Stage View](https://gitlab.com/mujtaba.qureshi/deploy-on-k8s/-/raw/main/Images/Jenkins-pipeline-view.jpg?ref_type=heads)

Version Increment In git repository by jenkins.

![Version Increment In git](https://gitlab.com/mujtaba.qureshi/deploy-on-k8s/-/raw/main/Images/Version%20Increment%20in%20Git%20repo%20.jpg?ref_type=heads)

Pushed Docker image In ECR.

![ECR Repo View](https://gitlab.com/mujtaba.qureshi/deploy-on-k8s/-/raw/main/Images/ECR-repo-view.jpg?ref_type=heads)

Deployed Application in Eks Cluster.

![Eks CLuster](https://gitlab.com/mujtaba.qureshi/deploy-on-k8s/-/raw/main/Images/Eks-Cluster-view.jpg?ref_type=heads)





