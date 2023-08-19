# docker_example

## 1. docker image build
  - docker build -t app-test .

## 2. docker image run
  - docker run --rm -p 8080:8080 app-test


# kubernetes_example

## 1. app deployment & service
  - kubectl apply -f kubernetes-deploy.yaml  (it need docker image files when it deploy)
  - kubectl get pods (get service on instances)
  - kubectl get nodes (get service nodes)
  - kubectl get services (get service associated load-balancer with public ip)

