# 1.17 Node.js development setup inside docker container

## Getting started

Pull the image from hub:

```
docker pull tomirantanen/node-dev-environment
```

Or build by yourself:

```
docker build -t node-dev-environment .
```

Run the image to start development environment.
Container is started with port 3000 exposed and project files are mounted as volume.

```
docker run --rm -it -p 3000:3000 -v $(pwd):/app tomirantanen/node-dev-environment
```

Install packages inside the container with npm:

```
npm install
```

Start node server:

```
npm run start:dev
```

App is now running on http://localhost:3000.
Open `index.js` in your favorite editor and start coding. Nodemon will automatically restart the app when files are changed.
