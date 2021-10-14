# week1
### 第三课和第一课是同一个工程. 我使用自己搭建的docker进行了构建和镜像推送

### 操作步骤:
- 1.构建镜像
    - docker build -t pangmu/httpserver:v1 .
    
- 2.运行服务
    - docker run -p 9090:8080  pangmu/httpserver:v1
    
- 3.验证服务
    - curl localhost:9090/healthz