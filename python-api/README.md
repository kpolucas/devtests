
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
