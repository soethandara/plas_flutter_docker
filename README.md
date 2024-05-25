## Flutter Development Environment in Docker Container

1. ⚙️ [About the System](#1-about-the-system) 
2. 🔨 [Prerequisites](#2-prerequisites) 
3. 🖥 [Follow the procedure according to OS](#3-procedure-according-to-OS) 
	- [Windows](#windows)
	- [Linux (Ubuntu)](#linux-Ubuntu)
	- [MacOS](#macos)
		- [Intel Processor](#macos-intel-processor)
		- [M1/2/3 Chip Processor](#macos-m-chip-processor) 
4. 📜 [About Exercises](#4-about-exercises) 
	- [Exercise-1](#exercise-1)
	- [Exercise-2](#exercise-2)
	- [Exercise-3](#exercise-3)
5. 📑 [Answer File](#5-answer-file) 
6. 🔖 [Answer File Submission Links](#6-answer-file-submission-links) 
7. 📝 [System Usage Feedback](#6-system-usage-feedback) 

<hr style="border-top: 2px solid #333;">

## 1. About the System 
<p align="justify"> 
In response to the identified challenges confronted by students in mobile app development education, this study introduces a comprehensive solution with Docker containers. The background emphasizes the difficulties students encounter in setting up development environments for Flutter app development. Addressing this issue, our proposed system streamlines the entire process within a Docker container, thereby offering a hassle-free environment accessible through Visual Studio Code (VSCode) across diverse operating systems, including Windows, Linux, and Mac.
</p>

<p align="center">
  <img src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/0b143fce-8f8e-4fe4-b8b4-7d748595ee75" alt="flutter" width="800" />
</p>
<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>

<hr style="border-top: 2px solid #333;">

## 2. Prerequisites 
- It is needed to install <strong>VSCode</strong> and <strong>Docker</strong>. Then, three extensions (flutter, remote development, docker) are necessary to add. <strong>if necessary,</strong> please download & reference the following user manual [plas_flutter_docker.pdf](https://github.com/soethandara/plas_flutter_docker/files/13625155/plas_flutter_docker.pdf)

	|                                                        Tool                                                        | Install | URL                                                                                                     |
	| :---------------------------------------------------------------------------------------------------------------------------: | :-------------: | ------------------------------------------------------------------------------------------------------- |
	| <img height="50" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/15f6e72c-eb4d-4704-b6e8-1d2002625c6a"> |      VSCode       | <ul><li>https://code.visualstudio.com/</li></ul> |
	| <img height="50" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/74b958e4-8211-481c-8454-8aa7a719ce8b"> |      Docker       | <ul><li>https://www.docker.com/products/docker-desktop</li></ul>|
	| <img height="50" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/3c890766-dda1-4b84-80b2-57ae170f6e40"> |      flutter       | <ul><li>`Add 'flutter' extension to VSCode`</li></ul> |
	| <img height="50" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/54ff3a0b-46cc-442e-9e4f-d5df90509cb4"> |      remote development       | <ul><li>`Add 'remote development' extension to VSCode`</li></ul> |
	| <img height="50" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/74b958e4-8211-481c-8454-8aa7a719ce8b"> |      docker       | <ul><li>`Add 'docker' extension to VSCode`</li></ul> |

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

## 3. Procedure according to OS
- Depending on the Operating System, the way is different. Therefore, please follow the procedure according to the conrrespondence OS.
##
### Windows

> **Get** the docker image, which has flutter development environment.
```
docker pull soethandara/plas_flutter_docker:v1.1
```

> **Get** the project from Github, which has
- docker-compose.yml to execute pulled docker image
- devcontainer.json to connect running docker container from VSCode.
```
git clone https://github.com/soethandara/plas_flutter_docker.git
```

> **Open** VSCode and correspondence folder **plas_flutter_docker/windows/**

> **Connect** to container
  - **Click** <img width="33" alt="Screenshot 2023-10-26 at 22 41 49" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/67707f4d-ba87-464d-abad-31421b524253">
 ```icon at the left-button of VSCode```
  - **Type**  ```Reopen in Container ``` (or) **Choose**  ```Open Folder in Container...```

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑</a>
<hr style="border-top: 2px solid #333;">

### Linux (Ubuntu)

> **Get** the docker image, which has flutter development environment.
```
docker pull soethandara/plas_flutter_docker:v1.1
```

> **Get** the project from Github, which has
- docker-compose.yml to execute pulled docker image
- devcontainer.json to connect running docker container from VSCode.
```
git clone https://github.com/soethandara/plas_flutter_docker.git
```
 
> **Open** VSCode and correspondence folder **plas_flutter_docker/linux/**

> **Connect** to container
  - **Click** <img width="33" alt="Screenshot 2023-10-26 at 22 41 49" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/67707f4d-ba87-464d-abad-31421b524253">
 ```icon at the left-button of VSCode```
  - **Type**  ```Reopen in Container ``` (or) **Choose**  ```Open Folder in Container...```

> [!CAUTION]
> if **error** is occurred in the above stage, please do the following:
- **Click** ```Edit devconainer.json Locally```
- **Open** terminal from VSCode
- **Type** the following
```
docker compose up
```

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑</a>
<hr style="border-top: 2px solid #333;">

### MacOS
> Apple's transition from Intel processors to its custom-designed chips (M1/2/3), starting with the M1 and subsequent iterations. Before their transition, Apple Mac computers used Intel processors. It is provided for both Intel and M chip processors.
##
### MacOS (Intel Processor)

> **Get** the docker image, which has flutter development environment.
```
docker pull soethandara/plas_flutter_docker:v1.1
```

> **Get** the project from Github, which has
- docker-compose.yml to execute pulled docker image
- devcontainer.json to connect running docker container from VSCode.
```
git clone https://github.com/soethandara/plas_flutter_docker.git
```

> **Open** VSCode and correspondence folder **plas_flutter_docker/mac/intel/**

> **Connect** to container
  - **Click** <img width="33" alt="Screenshot 2023-10-26 at 22 41 49" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/67707f4d-ba87-464d-abad-31421b524253">
 ```icon at the left-button of VSCode``` 
  - **Type**  ```Reopen in Container ``` (or) **Choose**  ```Open Folder in Container...```

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑</a>
<hr style="border-top: 2px solid #333;">

### MacOS (M Chip Processor)

> **Get** the docker image, which has flutter development environment.
```
docker pull soethandara/plas_flutter_docker:v1.2
```

> **Get** the project from Github, which has
- docker-compose.yml to execute pulled docker image
- devcontainer.json to connect running docker container from VSCode.
```
git clone https://github.com/soethandara/plas_flutter_docker.git
```

> **Open** VSCode and correspondence folder **plas_flutter_docker/mac/mchip/**

> **Connect** to container
  - **Click** <img width="33" alt="Screenshot 2023-10-26 at 22 41 49" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/67707f4d-ba87-464d-abad-31421b524253">
 ```icon at the left-button of VSCode``` 
  - **Type**  ```Reopen in Container ``` (or) **Choose**  ```Open Folder in Container...```

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑</a>
<hr style="border-top: 2px solid #333;">

## 4. About Exercises
> Student can see 3 sample flutter projects under **/root** directory using the following comment on VS code terminal. Students need to modify these 3 sample projects according to the expected results. If above step-3 is successful, it will automatically enter to the running container and terminal will be opened. The following things can be performed at the opened terminal.

```
ls -al /root
```
##
### Exercise-1

> **Copy** the exercise-1 to workplace
```
scp -r /root/exercise1 /root/workspace/
cd /root/workspace/exercise1
```
> **Modify** the codes as same as **expected result** in **main.dart** under **lib folder** from exercise-1 
      
![e1](https://github.com/soethandara/plas_flutter_docker/assets/148550611/69159920-c512-46f9-9245-5eb82764a35e)

> **Run** following command to check the output
```
flutter run -d web-server
```

> **Access** http://localhost:port

<img width="678" alt="autoPort" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/30f1159c-a36b-465c-be39-049ead64c822">

(**port number** is dynamic and so, access url will be displayed in the output of above command. It can be accessed then.)

> [!CAUTION]
> On **MacOS**, there may have no response matter, when calling the url (http://localhost:port). If so, use the following command
```
flutter run -d web-server --web-hostname 0.0.0.0 --web-port 5001
```

> **Access** http://localhost:5001

<img width="984" alt="setPort" src="https://github.com/soethandara/plas_flutter_docker/assets/148550611/c6f3c39a-5894-4ff4-bb10-000ae2155e66">

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

### Exercise-2

> **Copy** exercise-2 to workplace
```
scp -r /root/exercise2 /root/workspace/
cd /root/workspace/exercise2
```
> **Modify** the codes as same as **expected result** in **main.dart** under **lib folder** from exercise-2
      
![e2](https://github.com/soethandara/plas_flutter_docker/assets/148550611/d0d846d0-c863-4c7c-8c30-340b743fca78)

> **Run** to check the output
```
flutter run -d web-server
```

> **Access** http://localhost:port

(**port number** is dynamic and so, access url will be displayed in the output of above command. It can be accessed then.)

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

### Exercise-3

> **Copy** exercise-3 to workplace
```
scp -r /root/exercise3 /root/workspace/
cd /root/workspace/exercise3
```
> **Modify** the codes as same as **expected result** in **main.dart** under **lib folder** from exercise-3 
   
![e3](https://github.com/soethandara/plas_flutter_docker/assets/148550611/b9e04973-89c6-4518-97d0-7665b652b342)

> **Run** to check the output
```
flutter run -d web-server
```

> **Access** http://localhost:port

(**port number** is dynamic and so, access url will be displayed in the output of above command. It can be accessed then.)

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

### Exercise-4

> **Copy** exercise-4 to workplace
```
scp -r /root/exercise4 /root/workspace/
cd /root/workspace/exercise4
```
> **Modify** the codes as same as **expected result** in **main.dart** under **lib folder** from exercise-4
      
![e4](https://github.com/soethandara/plas_flutter_docker/assets/148550611/8a6689c2-8582-478b-ae38-20aa37c63a5b)

> **Run** to check the output
```
flutter run -d web-server
```

> **Access** http://localhost:port

(**port number** is dynamic and so, access url will be displayed in the output of above command. It can be accessed then.)

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

### Exercise-5

> **Copy** exercise-5 to workplace
```
scp -r /root/exercise5 /root/workspace/
cd /root/workspace/exercise5
```
> **Modify** the codes as same as **expected result** in **main.dart** under **lib folder** from exercise-5
      
![e5](https://github.com/soethandara/plas_flutter_docker/assets/148550611/399eb8ae-61d1-47db-99e3-d65deb51e171)

> **Run** to check the output
```
flutter run -d web-server
```

> **Access** http://localhost:port

(**port number** is dynamic and so, access url will be displayed in the output of above command. It can be accessed then.)

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

## 5. Answer File
> Student need to submit **main.dart** for each exercise and the location of **main.dart** (for e.g. exercise1 in below)
- ```C://flutter_workspace/exercise1/lib/main.dart```  at **Windows**
- current_directory```/exercise1/lib/main.dart```  at **Linux**
- current_directory```/exercise1/lib/main.dart```  at **MacOS**
 
<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

## 6. Answer File Submission Links
> To submit **main.dart**, rename as the following format.
  - **studentId_main.dart** (e.g, 43M21510_main.dart)

- **📜 Exercise1**
 https://u.pcloud.com/#page=puplink&code=7XIkZ3rfLz7YXcmYlTj1QtJ9nA01IEKB7

- **📜 Exercise2**
 https://u.pcloud.com/#page=puplink&code=kXIkZ6Ye4qeJJqihxtKHtTxDJgmOaNYdy

- **📜 Exercise3**
 https://u.pcloud.com/#page=puplink&code=XXIkZi84JJaLos9LMkftECB3iFp8skIR7

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑ </a>
<hr style="border-top: 2px solid #333;">

## 7. System Usage Feedback
> Please access the following **Google form** for taking survey usage of this system
  
- 📝 https://forms.gle/hidR2kpiEtAQJ2uJ6

<a href="#flutter-development-environment-in-docker-container" style="font-size: 0.1px; color: #FF0000;">if back to top ↑</a>
<hr style="border-top: 2px solid #333;">
