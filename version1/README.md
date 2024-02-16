Understanding the Project
​
🔐
Docker ID
This is basically your docker hub account username. Create an account  
Try a sample container
docker pull sampson101/web-app 
docker run –d –p 900:80 sampson101/web-app 
browse http://localhost:900 
​
☕
 Creating the Project files
On your computer Create a project folder with a name of your choice, let's say "docker-web-app". 
 Inside the project folder, create two sub-folders named "version1" and "version2".
*it is recommended to set up your git version control at the start.


Version 1: project
Your main outcome is to have a shareable working docker image hosted on the docker Hub
​
📂
 Project Files
Create a simple HTML file named "index.html" inside the "version1" folder. The HTML file will be a basic login form you would like to display. 
* static webpage
Create a Dockerfile in the "version1" folder. Dockerfiles are what tell docker how it should build your image (environments). thorough research is needed
​
Build first custom docker image
Using an online terminal or local. Ensure you are able to access your project files
Run the build commands
Ensure you can see your new custom image (docker images)
Run the Image to confirm it works
Finally, If all is right, let's push the image to a docker Hub repo
 To Note
Ensure you have a static login webpage
Ensure you have repos on GitHub and docker hub


SOLUTION STEPS

1. created our index.html file from the existing sample given.
2. created the main working directory and its sub folders version1 and version2
3. initiated the versioniong command in the folder git init
4. created the Dockerfile and Josh got as the image code
5. it was files were added, commited to git
6. Build the image [docker build -t kali .] //kali is the name of the image
7. To see the images created [dockker images]
8. Run the image to create a container [docker run -d -p 8089:80 --name KaliWeb kali]
9. To see the container [docker ps]
# Login to the webpage with the URL
10. Login to the docker Hub on the terminal [docker login]
11. We have to push to docker hub but we have to tag it first [docker tag kali loompesky/kali]
12. docker push loompesky/kali
13. Create a repo in github and then git remote it