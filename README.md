# prime-voting-app
Microservice app deployed on K8s. 
To Run on your local machine:
  - Start minikube: minikube start
  - Download the repository to your local machine: git clone https://github.com/bosphoran/prime-voting-app.git
  - Go to the foler prime-voting-app: cd prime-voting-app
  - Run the .YAML files in this order:
        - kubectl create -f voting-app-deploy.yaml
        - kubectl create -f voting-app-service.yaml
        - kubectl create -f redis-deploy.yaml
        - kubectl create -f redis-service.yaml
        - kubectl create -f postgres-deploy.yaml
        - kubectl create -f postgres-service.yaml
        - kubectl create -f worker-app-deploy.yaml
        - kubectl create -f result-app-deploy.yaml
        - kubectl create -f result-app-service.yaml

Note: If you want to deploy the app on the cloud. Then, change the type in the spec section to LoadBalancer instead to NordPort.
