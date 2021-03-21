# GGJAM Backend
This is the Dockerfile for [ghost-s3](https://hub.docker.com/r/wunderhund/ghost-s3), a Docker container for the [Ghost](https://ghost.org/) CMS that incldues an [S3 storage adapter](https://ghost.org/integrations/amazon-s3/) for simple storage of images on an AWS S3 bucket. I created this as the backend for a sample blog infrastructure I built, which can be found in the [ggjam](https://github.com/wunderhund/ggjam) repo.

This repo also incldues a docker-compose file to be used in combination with my customized Gatsby static site generator in my [ggjam-frontend](https://github.com/wunderhund/ggjam-frontend) repo.
This is designed to be used as an offline blogging solution. 

To run Ghost locally with this repo:
1. Run `docker-compose up -d`
1. In your browser, go to `http://localhost:2368/ghost` and set up a username and password.
1. Begin blogging!

Ghost is designed to serve a blog directly: you can see the blog itself at `http://localhost:2368`. But I prefer to serve static sites on the Internet, and you can run a static site generator like Gatsby against Ghost's API to generate site files, and then upload them to your public-facing storage or web server. If you're interested in using a Gatsby static site generator for this purpose, see my [ggjam-frontend](https://github.com/wunderhund/ggjam-frontend) repo.

To learn more about the versatile Ghost CMS, check out their site: [ghost.org](https://ghost.org/).