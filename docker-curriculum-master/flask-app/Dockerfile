## This is docker syntax that is run when the command "docker run" is run. 

#specify image to use
FROM python:3.8

#set up workign directory for the app
WORKDIR /usr/src/app

#COPY all files to the container we are creating 
COPY . .

#install dependencies using the requirements.txt as a template for everything needed
RUN pip install --no-cache-dir -r requirements.txt

#Specify port to be exposed, choose 5000 because thats what their flask app is setup to use
EXPOSE 5000

#command to actually run the APP, from the directory. this will run "python ./app.py". each word is seperated as its own element in an array
CMD ["python", "./app.py"]