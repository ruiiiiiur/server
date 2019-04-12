## **A NodeJS Server**

##### What is a NodeJS Server?

**[NodeJS](https://github.com/nodejs) is an open source server framework. In this project, a NodeJS server is used to save questions created by Question Setting App to the database using JavaScript. These questions are then served to the Quiz App and displayed on the map. When users answer questions in Quiz App, answers are saved to the database.**

##### System requirements

**Software**: An SSH file transfer system is needed.

- > For Mac: Fugu [1.2.1pre1](http://sourceforge.net/projects/fugussh/files/Unstable/fugu-1.2.1pre1/Fugu-1.2.1pre1.zip/download). (Download link: http://rsug.itd.umich.edu/software/fugu/)

- > For Windows: BitVise Client [8.29](https://www.bitvise.com/ssh-client-download) (Download link: https://www.bitvise.com/ssh-client-download)

##### How to run the server

1. Clone the server

   ```
   cd code
   
   git clone https://github.com/ucl-geospatial/ucesrji-server.git
   ```

2. Switch off the existing servers

   ```
   pm2 list
   
   pm2 stop 0/1/2/...
   ```

3. Start the server created for this app

   - Debug mode (error messages are visible)

   ```
         cd code/ucesrji-server
         node myServer.js
   ```

   - Or keep the server running permanently (error messages are not visible)

   ```
         cd code/ucesrji-server
         pm2 start myServer.js
   ```

