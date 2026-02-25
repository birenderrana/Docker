#Choose the base image 
FROM python:3.10-alpine

#Create a workdir inside the docker container
WORKDIR /app

#COPY the requirement file to container working dir /app
COPY requirement.txt .

#Run the requirement file inside the container
RUN pip install --no-cache-dir -r requirement.txt

#COPY rest of the code.  
COPY . .

#Run the python code
CMD ["python" , "app.py"]