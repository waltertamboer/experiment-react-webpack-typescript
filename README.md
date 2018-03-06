# experiment-react-webpack-typescript

Run a ReactJS application compiled with Webpack and Typescript.

Tutorial described here: https://www.typescriptlang.org/docs/handbook/react-&-webpack.html

## Installation

Install the dependencies.

```
docker run --rm -it -v $(pwd):/data -w /data node npm install
docker run --rm -it -v $(pwd):/app jmfirth/webpack webpack
```

Run the webserver:

```
docker-compose up -d
```

## What's happening

Webpack bundles the TSX files (http://www.typescriptlang.org/docs/handbook/jsx.html) 
into a JavaScript bundle. This bundle is loaded in the index file which basically loads
the application.

