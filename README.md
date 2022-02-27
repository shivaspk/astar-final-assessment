# Astar-final-assessment
This is prerequisite for Final Assessment

Please follow the below steps to setup the inital environment

# To install Kong Ingress Controller with Helm 3

`$ helm repo add kong https://charts.konghq.com`

`$ helm repo update`

`$ helm install kong/kong --generate-name --set ingressController.installCRDs=false`

# To Create Deployments and Ingress
`kubectl apply -f .\customerdeploy.yaml -f .\inventorydeploy.yaml -f .\productdeploy.yaml -f .\ingress.yaml`

# To run RabbitMQ
`kubectl apply -f .\rabbitmqdeploy.yaml`

# To run MS SQL Statefulset
`kubectl apply -f .\mssqlsts.yaml`

# To run Metrics Server
`kubectl apply -f .\metrics-server.yaml`

# To make your editing better
Use Visual Studio 2019/2022 for Development 

Use Visual Studio Code for editing with following Plugins:

1) Docker 
2) Kubernetes
3) Live Server (for HTML)

Tips

1) All the JS code that needs to be edited is in `js` folder named `common.js`
2) Try to complete maximum number of tasks