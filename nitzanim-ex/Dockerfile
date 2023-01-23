#if the new image is right this should work
FROM python:3.12-rc-bullseye

# Set the working directory
WORKDIR /app

# Using the right environment variables
ENV FLASK_APP=flaskr
ENV FLASK_ENV=development

# Copy the files
COPY . .

# Install the dependencies
RUN pip install --editable . && flask init-db

# exposing port 
EXPOSE 5000

# Running? please?
CMD ["flask", "run", "--host=0.0.0.0"]