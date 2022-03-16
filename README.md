# docker_android_studio
Android Studio Docker container can be run on the server. User can use Android Studio via ssh with authorized access without installing it on their own PC.
It will be useful for the user who doesn't have enough computing power to start Android Studio.
___________________________________________________________________________________________________________________________________________________

### Prerequisite for User
```
1. It is needed to install ssh client to access the server.
2. Then, user will reach to the server of the permitted session.
3. User can run the following.
    >>cd docker_android_studio/
    >>HOST_DISPLAY=1 ./run.sh
4. Android Studio will be started.
```
___________________________________________________________________________________________________________________________________________________

### Prerequisite for Server Administrator
```
It is needed to install Docker. Then,
>>docker pull pollen5005/android_studio_hh:v1
```

### Setting the project for User
```
1. git clone (or) download the project zip 
2. put the project under each user session of the server.
```
___________________________________________________________________________________________________________________________________________________
### Workflow Design
![hein_docker(1)](https://user-images.githubusercontent.com/79504426/158392451-db89cbb2-b84f-4f67-a989-f54559a483b2.png)
___________________________________________________________________________________________________________________________________________________
### User Manual (for current testing)
1. Install Docker on Server
2. Pull the Docker image from Docker Hub using the following command:
>>docker pull pollen5005/android_studio_hh:v1
3. Download the project from GitHub
>>git clone https://github.com/upc-hub/docker_android_studio
4. Change the directory to the downloaded project
5. Run the shell file using the following command:
>>HOST_DISPLAY=1 ./run.sh
6. Finally, it will open the Android Studio for creating the android project.

### User Manual (for the next testing)
1. Create space for each student at server (add new user in server)
2.  Under each space, put the project downloaded from GitHub
3. Student can access designated space via ssh 
(eg. ssh hein@114.6.25.185)
4. After student reached to the server, only the following script is needed to run.
 >>HOST_DISPLAY=1 ./run.sh
___________________________________________________________________________________________________________________________________________________

