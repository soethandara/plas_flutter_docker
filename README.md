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

4. Open VS Code manually or type```code .``` from terminal

5. Connect to container
  - Click <img width="33" alt="Screenshot 2023-10-26 at 22 41 49" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/67707f4d-ba87-464d-abad-31421b524253">
 ```icon at the left-button of VSCode``` (or) ```shift+alt+p ```
  - Type -> ```Open Folder in Container...``` (or) ```Reopen in Container ```

### Goals
- **Student can see sample flutter projects to check the system is working correctly or not**
  - go to each project
  - run ```flutter run -d web-server```
- **Student can also create his/her own flutter app**
  - create project
    - ```mkdir sample_project_1```
    - ```cd sample_project_1```
    - ```flutter create .```    
