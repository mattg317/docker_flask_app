# Running your flask app with docker

1. Sign up for account on [Docker Hub](https://hub.docker.com/)

2. Build the image `docker build -t <username>/<imagename> .`

3. Run the image `docker run -p 8888:5000 <username>/<imagename>`

4. Navigate to `localhost:8888` to view your website.