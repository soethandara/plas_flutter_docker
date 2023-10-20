# Flutter Development Environment in Docker Container
![flutter](https://github.com/soethandara/plas_flutter_docker/assets/148550611/26af9f16-4306-47be-ac17-36ad895f4185)

## Prerequisites 
- install **VSCode**
- add the following extensions to VSCode
  - **Flutter, Docker, Remote Environment**
- install **Docker**
  
## System Usage
1. get the docker image, which has flutter development environment. 
```
docker pull soethandara/flutter_env_vscode
```

2. get the project from Github, which has
- **docker-compose.yml** to execute pulled docker image
- **devcontainer.json** to connect running docker container from VSCode.
```
git clone https://github.com/soethandara/plas_flutter_docker.git
```
- **For Windows user,**
  - go to windows folder
  - ```cd plas_flutter_docker/windows/```
- **For MacOS user,**
  - go to mac folder
- **For Linux user,**
  - go to linux folder
- Open VS Code
- Connect to container
  - Click >< icon at the left-button of VSCode (or) shift+alt+p 
  - Type -> Open Folder in Container...
- Student can see sample flutter projects
  - go to each project
  - run "flutter run -d web-server"
- Student can create own flutter app
  - create project
    - mkdir sample_project_1
    - cd sample_project_1
    - flutter create .    
