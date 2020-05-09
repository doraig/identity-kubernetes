# identity-kubernetes
Simple two pod IS deployment using kubernetes

# STEPS

1) kubectl apply -f identity-namespace.yaml
2) kubectl apply -f identity-svc.yaml
3) kubectl apply -f identity-server-conf.yaml
4) kubectl apply -f identity-wso2is-service.yaml
5) kubectl apply -f identity-server-ingress.yaml
6) kubectl apply -f identity-server-deployment.yaml

Kubectl version : v1.18.1
Minikube version : 1.7.3

If you are using minikube To enable the NGINX Ingress controller, run the following command:

minikube addons enable ingress

Add wso2is <minkube ip> to /etc/hosts

https://wso2is/carbon/admin/login.jsp