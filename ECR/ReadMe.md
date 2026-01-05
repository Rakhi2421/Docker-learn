# AMAZON ECR

## Docker Registry

- Docker private repository
- Registry Options
- Build & Tag an image
- docker login
- docker push
---

#### Create Private docker repository on AWS  

ECR (Elastic Container Registry)  

- Login to AWS Console --> Search ECR --> Get-Started --> Name Repository --> Click create Repository.

- Use a seperate repository per image.
- You always have to login to private repo using docker login command.
- In aws ecr you can find the commands how to push an image to ECR.

## Image Naming in docker registries

registrydomain/imagename:tag  

In Docker Hub:  
>when we run docker pull mongo:4.2   

>it works as : docker pull docker.io/library/mongo:4.2  

In AWS ECR:  
> docker pull 520697001743.dkr.ecr.eu-central-1.amazon.aws.com/myapp:1.0  
- If you want to push a local image(myapp:1.1) to ECR 
> docker tag myapp:1.1 520697001743.dkr.ecr.eu-central-1.amazon.aws.com/myapp:1.1
> docker push myapp:1.1 520697001743.dkr.ecr.eu-central-1.amazon.aws.com/myapp:1.1

