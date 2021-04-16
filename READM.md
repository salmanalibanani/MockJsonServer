docker build -t mockbackend .
docker run -d -p 8080:8080 --name mb1 mockbackend

- From your localhost:

curl 127.0.0.1:8080/posts/1

- Test the container interactively.

docker exec -it mb1 bash
curl 127.0.0.1:8080/posts/1
