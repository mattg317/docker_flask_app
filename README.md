# Running your flask app with docker

1. Sign up for account on [Docker Hub](https://hub.docker.com/)

2. Builder the image `docker build -r <username>/<imagename> .`

3. Run the image `docker run -p 8888:5000 <username>/<imagename>`

4. Navigate to `localhost:8888` to view your website.