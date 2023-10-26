# Flutter Development Environment in Docker Container
![flutter](https://github.com/soethandara/plas_flutter_docker/assets/148550611/26af9f16-4306-47be-ac17-36ad895f4185)

## Prerequisites 
- install **VSCode**
- add the following extensions to VSCode
  - **Flutter, Docker, Remote Environment**
- install **Docker**
  
## System Usage
1. get the **docker image**, which has **flutter development environment**. 
```
docker pull soethandara/plas_flutter_docker:v1
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

4. Type```code .``` from terminal (or) Open VS Code and correspondence folder manually according to your OS (eg. plas_flutter_docker/windows)

6. Connect to container
  - Click <img width="33" alt="Screenshot 2023-10-26 at 22 41 49" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/67707f4d-ba87-464d-abad-31421b524253">
 ```icon at the left-button of VSCode``` (or) ```shift+alt+p ```
  - Type -> ```Open Folder in Container...``` (or) ```Reopen in Container ```

### Goals
- **Student can see three sample flutter projects under /root directory**
  - ls -al /root
- **Student can modify these three sample projects according to the guide document as the exercise**
  - **Exercise1**
    - scp -r /root/exercise1 .
    - modify the codes from VSCode
    - **Output in sample project**
      - ![e1-1](https://github.com/soethandara/plas_flutter_docker/assets/148550611/b5d161b5-a06c-4f94-b70e-00be93a89818)
    - **Expected result**
      - 
    - run ```flutter run -d web-server```
  - **Exercise2**
    - scp -r /root/exercise2 .
    - modify the codes from VSCode
    - **Output in sample project**
    - **Expected result**
    - run ```flutter run -d web-server```
  - **Exercise3**
    - scp -r /root/exercise3 .
    - modify the codes from VSCode
    - **Output in sample project**
    - **Expected result**
    - run ```flutter run -d web-server```
      
- **Student can also create his/her own flutter app**
  - create project
    - ```mkdir sample_project_1```
    - ```cd sample_project_1```
    - ```flutter create .```
    - write flutter app
    - test output by ```flutter run -d web-server```

### Feedbacks
- Please access the following **Google form** for taking survey usage of this system
