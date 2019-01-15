# this dockerfile installs the Apollo GraphQL server based on the demo from this link
# https://www.apollographql.com/docs/apollo-server/getting-started.html#Step-1-Project-initialization

# ----------------------------------
# STEPS
# ----------------------------------
# STEP 1 - build docker image
# docker build --tag apollo .;docker run --rm -it apollo bash
# STEP 2 - run docker image
# once the docker image is build from STEP 1, exit the running docker image
# then run the newly built docker image with parameters to expose the console port 4000
# docker run -it -p 4000:4000 apollo bash
# STEP 3 - start apollo server
# node index.js
# STEP 4 - open the apollo console from browser
# http://localhost:4000/
# STEP 5 - perform apollo console query
# paste the following into the apollo console
# { books { title author } }

FROM ubuntu:latest

# ----------------------------------
# install supporting applications
# ----------------------------------
RUN apt-get update && apt-get install -y git && apt-get install -y npm && apt-get install -y curl && apt-get install -y vim && npm i -g npx

# ----------------------------------
# install apollo server & graphql
# ----------------------------------
COPY index.js /index.js
RUN npm init --yes
RUN npm install --save apollo-server graphql

EXPOSE 4000:4000

