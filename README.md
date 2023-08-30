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
![image](https://github.com/khkwon01/docker_kubernetes/assets/8789421/575390fd-c242-4002-b25c-bff8dfaa9234)

![image](https://github.com/khkwon01/docker_example/assets/8789421/c411bbaf-7e48-4444-ae42-abba2411c66d)

![image](https://github.com/khkwon01/docker_example/assets/8789421/4d7104ab-0ab5-481b-967f-8fd0fcb2f30d)
![image](https://github.com/khkwon01/docker_kubernetes/assets/8789421/2d528bc3-03a7-4389-be83-d8704a6c2fe0)

  - Volume    
    ![image](https://github.com/khkwon01/docker_kubernetes/assets/8789421/56bd1348-61df-44a7-9a1b-7c32034b26e2)

  - PesistentVolume     
    ![image](https://github.com/khkwon01/docker_kubernetes/assets/8789421/3e199de6-69da-4c7a-816e-22fd3323e30c)
    ![image](https://github.com/khkwon01/docker_kubernetes/assets/8789421/907fec7a-2c19-4ca4-a2d1-f3a1ee87a9ee)


## 1. app deployment & service
  - kubectl apply -f kubernetes-deploy.yaml  (it need docker image files when it deploy)
  - kubectl get pods (get service on instances)
  - kubectl get nodes (get service nodes)
  - kubectl get services (get service associated load-balancer with public ip)
    - provide load-balanced access to specified pods (cluster IP, nodeport, load-balancer)
  - kubectl get persistentvolumeclaim
    - deploy : kubectl apply -f pvc-disk.yaml
  - kubectl exec -it <<Pod Name>> -- sh
  - kubectl describe <<Pod Name>>

## 2. Deployment
### 1. Blue/Green Deployment
- Overall archectiture
  ![image](https://github.com/khkwon01/docker_example/assets/8789421/154275ef-4384-4fd0-b006-53d9a4ed5713)
- How to setup
  ![image](https://github.com/khkwon01/docker_example/assets/8789421/aa6de144-4090-4f84-9f84-4ca7a533b2b0)


### 2. Canary Deployment
- Overall archectiture
  ![image](https://github.com/khkwon01/docker_example/assets/8789421/c8b84ce3-a448-48dc-80d6-4715efa2fbfc)  

- How to setup    
  ![image](https://github.com/khkwon01/docker_example/assets/8789421/6c1b83fb-1ec8-4d51-8d89-ebd7047686b8)
