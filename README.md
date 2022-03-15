# docker_android_studio
Android Studio Docker container can be run on the server. User can use Android Studio via ssh with authorized access without installing it on their own PC.
It will be useful for the user who doesn't have enough computing power to start Android Studio.

### Prerequisite for User
```
1. It is needed to install ssh client to access the server.
2. Then, user will reach to the server of the permitted session.
3. User can run the the following.
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

### How to get the project
```
1. git clone (or) download the project zip 
2. put the project under each user session of the server.
```

### Workflow Design
![hein_docker(1)](https://user-images.githubusercontent.com/79504426/158392451-db89cbb2-b84f-4f67-a989-f54559a483b2.png)
