www.play-with-docker.com<br>

# docker build & run
`cd ~/docker/demo-apollo-graphql;docker build --tag apollo .`<br>
`docker run -it -p 4000:4000 apollo bash`<br>
`node index.js`<br>
paste this into the left side of console & press play button: <br>
`{ books { title author } }`<br>
this will perform a specific local query on title & author against that data set<br>




