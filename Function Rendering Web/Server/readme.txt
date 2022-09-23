o start a local web server that serves the index.html do the following steps:

Navigate into the folder in the command line, where the index.html is located.
Run npm init, it will ask some questions what configurations do you want to have in your package.json. If you are not sure yet, just go for the default values, you will be able to change them later.
Run npm install http-server --save-dev to have http-server as development dependency, which is able to serve the index.html file.
In package.json add to the scripts the start npm script for starting of the http-server: "scripts": {"start": "http-server"}.
Run npm start from the command line, the server will be started by default on http://localhost:8080/
Of course it is worth to put the html, css and js files in a separate folder, to serve them from that folder check the parameters of http-server.