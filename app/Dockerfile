#Get the official Python Base Image from Docker Hub.
FROM python

#In the image, create a directory named app.
RUN mkdir /app

#Set the working directory to that new app directory.
WORKDIR /app

#Copy the local directory’s contents to that new folder into the image.
ADD . /app/

#Run the pip installer to pull the requirements into the image.
RUN pip install -r /app/requirements.txt

#Inform Docker the container listens on port 5000.
EXPOSE 5000

#Configure the starting command to use when the container starts.
CMD ["python", "/app/app.py"]
