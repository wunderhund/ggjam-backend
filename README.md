# ggjam-backend
docker-compose backend for using ggjam locally

This runs a Ghost and a MySQL container locally, primarily used for testing my gatsby frontend located at https://github.com/wunderhund/ggjam-frontend. Can also be used as an offline blogging solution; write blog posts in Ghost, run a static site generator like Gatsby against it to generate the site, and then upload to your public-facing storage or web server.

To run, simply `docker-compose up`

Then access Ghost at http://localhost:2368/ghost/

