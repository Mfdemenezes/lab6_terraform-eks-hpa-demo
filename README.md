# lab6_terraform-eks-hpa-demo

Objetivo: EKS criado com Terraform + app com HPA (alvo 80% CPU).

Adicionar no terraform-eks-hpa-demo/README.md:

flowchart LR
    Terraform --> EKS[(AWS EKS)]
    EKS --> Deploy[Deployment]
    Deploy --> HPA[Horizontal Pod Autoscaler]
    HPA -->|escala| Pods[(Pods)]
    User((Usuário)) -->|Service| Deploy
