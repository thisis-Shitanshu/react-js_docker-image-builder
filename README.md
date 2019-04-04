# React JS Image builder

This project has **"react": "^16.8.3"**, which is used to build images for both Development and Production environment.

## Commands
After cloning the repository. Inside the project directory.

- Using Dockerfile.dev (Live load not enabled)
```
docker build -f Dockerfile.dev .
docker run -p 3000:3000 <IMAGE_ID>
```

*When using Docker Toolbox, pwd might not be supported. So, go to the VM settings and add current project directory to the shared folder.*
- Using Dockerfile.dev (Live load enabled)
```
docker run -p 3000:3000 -v /app/node_modules -v "<YOUR_CURRENT_DIRECTORY>":/app <IMAGE_ID>
```

- Using **docker-compose**
```
// Change your volume path in docker-compose.yml before running this command
$ docker-compose up
```