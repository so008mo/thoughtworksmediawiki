# thoughtworksmediawiki

This Project is to build a pipeline to deploy the media wiki helm chart to AWS EKS

Prerequisites to run the code

1. Linux Terminal
2. Docker
3. git

Steps to follow:

1. git clone https://github.com/so008mo/thoughtworksmediawiki.git

2. cd /thoughtworksmediawiki

3. docker build . -t arsenal14h/eks-utils       # The image is being pulled from my docker repository. The image is made public only for this project.

4. docker run -it arsenal14h/eks-utils /bin/bash  # The docker container has all the pre-installed executables needed to build this project.

5. cd /thoughtworksmediawiki

6. aws configure    # Please enter your secret access key and access id as per the AWS account that you want the project to be built.

7. ansible-playbook main.yml