# docker_example

## 1. docker image build
  - docker build -t app-test .

## 2. docker image run
  - docker run --rm -p 8080:8080 app-test

![image](https://github.com/khkwon01/docker_example/assets/8789421/2faba833-8733-4f99-87b9-4f9563d8e8eb)


# kubernetes_example
## 1. kubernetes basic architecture
![image](https://github.com/khkwon01/docker_example/assets/8789421/9308c96b-c203-4b3f-99f7-01f96c239908)
![image](https://github.com/khkwon01/docker_example/assets/8789421/8c32f270-3d8e-4099-9357-8e395f77bbc7)

![image](https://github.com/khkwon01/docker_example/assets/8789421/c411bbaf-7e48-4444-ae42-abba2411c66d)

![image](https://github.com/khkwon01/docker_example/assets/8789421/4d7104ab-0ab5-481b-967f-8fd0fcb2f30d)


## 1. app deployment & service
  - kubectl apply -f kubernetes-deploy.yaml  (it need docker image files when it deploy)
  - kubectl get pods (get service on instances)
  - kubectl get nodes (get service nodes)
  - kubectl get services (get service associated load-balancer with public ip)
    - provide load-balanced access to specified pods (cluster IP, nodeport, load-balancer)

