#Create a Docker image for React Start App.

This process mainly consists of two parts since this takes place only on a local server.
		1.Build
		2.Run
		
Use Docker Desktop for viewing the container logs.

###Build
First the Dockerfile.dev is used to build the docker image

docker build -f Dockerfile.dev -t mytag .

Note: The dot at the end is required too.


###Run
Then create the container using the docker image using the followinf command

docker run -d -it -rm -p 3001:3000 -name reactapp mytag

Then the container will be created and the react app can viewed on

https://localhost:3001

