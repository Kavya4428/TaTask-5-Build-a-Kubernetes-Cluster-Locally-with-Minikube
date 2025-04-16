# Task-5-Build-a-Kubernetes-Cluster-Locally-with-Minikube

# Kubernetes-Cluster-with-Minikube

Install Minikube on an Amazon EC2 instance using the `none` driver and deploying a simple NGINX app exposed via a `NodePort`.

## Prerequisites

- Amazon Linux EC2 instance (t2.medium or higher recommended)
- Docker installed and running
- Sudo/root access
- kubectl and Minikube binaries
  
## Installation and setup steps

1. Install `kubectl`
2. Install `Minikube` and dependencies
3. Start Minikube with none drive
4. Create `deployment.yaml` and `service.yaml`
5. Apply the configurations
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
6. Deploy `Kubectl`
kubectl get deploy
7. Check pod and service status
kubectl get pods
kubectl get svc nginx-service
8. Add  Security Groups
Ensure the following inbound rules in your EC2 security group:
Port 22 (SSH)
Port 80 (HTTP)
Port 32065 (NodePort)
Optional: Port Range 30000–32767 (for future NodePort services)
9. Access from browser/ ngnix-server
10. Cleanup
minikube delete
![Screenshot (134)](https://github.com/user-attachments/assets/1ebd7ca1-4875-4fc7-95ea-cc9f09b18254)
![Screenshot (136)](https://github.com/user-attachments/assets/389cbb76-f620-4d39-b089-99295338bf1a)
![Screenshot (137)](https://github.com/user-attachments/assets/10feb1d2-589d-474d-bd28-873c9e2aa238)
![Screenshot (139)](https://github.com/user-attachments/assets/c53eeaf8-dafa-434b-b27e-8d3e185edcae)
![Screenshot (140)](https://github.com/user-attachments/assets/dd9c5024-3dff-482b-b069-f931a19b65e1)
![Screenshot (142)](https://github.com/user-attachments/assets/4b9312c7-380f-4f6f-81cf-639c8ac14c5c)
![Screenshot (143)](https://github.com/user-attachments/assets/21919a6f-ab8e-40c2-ab33-b8a2490e6c12)


