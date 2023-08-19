# docker_example

## 1. docker image build
  - docker build -t app-test .

## 2. docker image run
  - docker run --rm -p 8080:8080 app-test

![image](https://github.com/khkwon01/docker_example/assets/8789421/2faba833-8733-4f99-87b9-4f9563d8e8eb)


# kubernetes_example

## 1. app deployment & service
  - kubectl apply -f kubernetes-deploy.yaml  (it need docker image files when it deploy)
  - kubectl get pods (get service on instances)
  - kubectl get nodes (get service nodes)
  - kubectl get services (get service associated load-balancer with public ip)

