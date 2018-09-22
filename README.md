# flask-hello-world

Bare-bones, not production-ready, Dockerized Flask.


## Example

```
$ docker build -t flask-hello-world .

$ docker run \
  --rm \
  -it \
  -v $(pwd):$(pwd) \
  -p 5000:5000 \
  -e FLASK_APP=$(pwd)/app/hello.py \
  flask-hello-world flask run --host=0.0.0.0
```
