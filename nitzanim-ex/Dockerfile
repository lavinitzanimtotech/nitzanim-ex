# if the new image is right this should work
FROM python:3.12-rc-bullseye

# set the working directory
WORKDIR /nitzanim-ex

# using the right environment variables
ENV FLASK_APP=flaskr
ENV FLASK_ENV=development

# copy 
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt 

# copy the files and initializa database
COPY . .
RUN flask init-db
 
# exposing port 
EXPOSE 5000

# running? please?
CMD ["flask", "run", "--host=0.0.0.0"]