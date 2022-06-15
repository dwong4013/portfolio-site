To build the docker image for development:
"docker build --target=development -t portfolio-site/development ."

To start the development container:
"docker run -p 3000:3000 -p 35729:35729 -e CHOKIDAR_USEPOLLING=true -e FAST_REFRESH=false -v <src-directory>:/usr/src/portfolio-site portfolio-site/development"