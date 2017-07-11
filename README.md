docker-bower
============

Runs `bower --allow-root --config.interactive=false install`  within a docker container

FROM node:alpine so its footprint is minimal, includes git

You can run a specific command like so 

    $ docker run -it -v "`pwd`":/data kzap/bower bash -c "bower --allow-root --config.interactive=false install [package name]"

