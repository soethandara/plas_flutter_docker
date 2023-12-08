# Flutter Development Environment in Docker Container
![flutter](https://github.com/soethandara/plas_flutter_docker/assets/148550611/26af9f16-4306-47be-ac17-36ad895f4185)
> [Go to Real Cool Heading section](#-real-cool-heading)
## Prerequisites 
- install **VSCode**
- add the following extensions to VSCode
  - **Flutter, Docker, Remote Development**
- install **Docker**
- **if necessary,** please reference the following user manual 
[plas_flutter_docker.pdf](https://github.com/soethandara/plas_flutter_docker/files/13191374/plas_flutter_docker.pdf)
  
## System Usage
1. get the **docker image**, which has **flutter development environment**.
- **For MacOS user,**   
```
docker pull soethandara/plas_flutter_docker:v1
```
- **For Windows/Linux user,**  
```
docker pull soethandara/plas_flutter_docker:v1.1
```

2. get the project from Github, which has
- **docker-compose.yml** to execute pulled docker image
- **devcontainer.json** to connect running docker container from VSCode.
```
git clone https://github.com/soethandara/plas_flutter_docker.git
```

3. go to the correspondence folder from the project
- **For Windows user,**
  - go to windows folder
  - ```cd plas_flutter_docker/windows/```
- **For MacOS user,**
  - go to mac folder
  - ```cd plas_flutter_docker/mac/```
- **For Linux user,**
  - go to linux folder
  - ```cd plas_flutter_docker/linux/```
  - ```docker compose up```

4. Type```code .``` from terminal (or) Open VS Code and correspondence folder manually according to your OS (eg. plas_flutter_docker/windows)

6. Connect to container
  - Click <img width="33" alt="Screenshot 2023-10-26 at 22 41 49" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/67707f4d-ba87-464d-abad-31421b524253">
 ```icon at the left-button of VSCode``` (or) ```shift+alt+p ```
  - Type -> ```Reopen in Container ``` (or) ```Open Folder in Container...```

## Goals
- **Student can see three sample flutter projects under /root directory using the following comment on VS code terminal**
  - ```ls -al /root```
- **Student can modify these three sample projects according to the guide document as the exercise**
  - **Exercise1**
    - ```scp -r /root/exercise1 .```
    - ```cd exercise1```
    - modify the codes as same as **expected result** in **main.dart** under **lib folder** from exercise1 
      
    ![e1](https://github.com/soethandara/plas_flutter_docker/assets/148550611/8b386cdb-117b-4625-acc3-4d66b535cc31)
    - run ```flutter run -d web-server```
  - **Exercise2**
    - ```scp -r /root/exercise2 .```
    - ```cd exercise2```
    - modify the codes as same as **expected result** in **main.dart** under **lib folder** from exercise2
      
    ![e2](https://github.com/soethandara/plas_flutter_docker/assets/148550611/187ade6d-4e35-4c25-8ce2-d627cecc7e0b)
    - run ```flutter run -d web-server```
  - **Exercise3**
    - ```scp -r /root/exercise3 .```
    - ```cd exercise3```
    - modify the codes as same as **expected result** in **main.dart** under **lib folder** from exercise3 
   
    ![e3](https://github.com/soethandara/plas_flutter_docker/assets/148550611/b8c49586-7b81-4af9-ba8a-7720b879837f)
    - run ```flutter run -d web-server```
      
- **Student can also create his/her own flutter app**
  - create project
    - ```mkdir sample_project_1```
    - ```cd sample_project_1```
    - ```flutter create .```
    - write flutter app
    - test output by ```flutter run -d web-server```

## Answer File Submission
- Student need to submit **main.dart** for each exercise
- Location of **main.dart**
    - ```C://flutter_workspace/exercise1/lib/main.dart``` at **Windows**
    - current_directory```/exercise1/lib/main.dart``` at **MacOS**
    - current_directory```/exercise1/lib/main.dart``` at **Linux**
  
- To submit **main.dart**, rename as the following format.
  - **studentId_main.dart** (e.g, 43M21510_main.dart)
- **Exercise1**
    https://u.pcloud.com/#page=puplink&code=7XIkZ3rfLz7YXcmYlTj1QtJ9nA01IEKB7
- **Exercise2**
    https://u.pcloud.com/#page=puplink&code=kXIkZ6Ye4qeJJqihxtKHtTxDJgmOaNYdy
- **Exercise3**
    https://u.pcloud.com/#page=puplink&code=XXIkZi84JJaLos9LMkftECB3iFp8skIR7

## System Usage Feedbacks
- Please access the following **Google form** for taking survey usage of this system
  https://forms.gle/hidR2kpiEtAQJ2uJ6

# Real Cool Heading
