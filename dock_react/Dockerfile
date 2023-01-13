## This is docker syntax that is run when the command "docker run" is run. 

#specify image to use
FROM node:16.14.0

#set up workign directory for the app
WORKDIR /usr/src/triumph_cake

#COPY all files to the container we are creating 
COPY . .

##DEPENDENCIES 

#install npm dependencies on image creation
RUN npm install


##Specify port to be exposed
#react server
EXPOSE 3000


#command to actually run the APP when docker run is started
CMD ["npm", "start"]