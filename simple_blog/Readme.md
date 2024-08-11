
docker build -t blogv .-- this will create an image

- This is to run docker file using volumes 
docker run --name blog_cv -p 4000:4000 -v d:/udemy/web_development/others/blog:/app -v /app/node_modules blogv:latest

- This is to run docker compse files

docker compose build -- this builds the image 
docker compose up -- this starts the container
docker compose down -- this stops the container
