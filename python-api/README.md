#### For test. Create, use venv, install deps
```
python3 -m venv venv
. venv/bin/activate
pip3 install flask flask-restful
```
#### To build/run the image
```
docker build --tag python-docker-luc .
docker run -d -p 5000:5000 python-docker
```

## flask API usage
#### To run api server
```
python api.py
```
#### To get list of tasks
```
curl http://localhost:5000/todos
```
#### To get single task
```
curl http://localhost:5000/todos/todo3
```
#### To delete a task
```
curl http://localhost:5000/todos/todo2 -X DELETE 
```
#### To add a new task
```
curl -H 'Content-Type: application/json' http://localhost:5000/todos -d '{"task":"something new"}' -X POST
```
#### To update a task
```
curl -H 'Content-Type: application/json' http://localhost:5000/todos/todo3 -d '{"task":"something different"}' -X PUT
```

#### Fuentes
https://www.freecodecamp.org/news/how-to-dockerize-a-flask-app/
https://flask-restful.readthedocs.io/en/latest/quickstart.html
