![1.PNG](/doc/1.PNG)

![2.PNG](/doc/2.PNG)

## LOGIN
```sh
curl -X POST http://127.0.0.1:8000/dj-rest-auth/login/ \
-H "Content-Type: application/json" \
-d '{"username": "user", "email": "user@example.com", "password": "user123$!A"}'
```

## LOGOUT
```sh
curl -X POST http://127.0.0.1:8000/dj-rest-auth/logout/ -H "Content-Type: application/json" --cookie "access=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoiYWNjZXNzIiwiZXhwIjoxNzI4ODQ0MzgxLCJpYXQiOjE3Mjg4NDQwODEsImp0aSI6ImMzOTU0OWNhYjJiMjQ1Zjk5MWQxOTIzMWFkY2VmYTUzIiwidXNlcl9pZCI6NH0.pohLBwqEhZ5ZBwWbOoKzkqQkl8XDKyzLJ5I7ThE9DaI; Path=/; HttpOnly; SameSite=Lax" --cookie "refresh_token=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ0b2tlbl90eXBlIjoicmVmcmVzaCIsImV4cCI6MTcyODkzMDQ4MSwiaWF0IjoxNzI4ODQ0MDgxLCJqdGkiOiIxOTI1ZDhmODgzYjc0YTQwYWM4ZGYzMjIyYjExMmM4YiIsInVzZXJfaWQiOjR9.ndVz0vbq2883Fo3njQFe6ae6bY_pkly-DmKZdgN0WEA; Path=/; HttpOnly; SameSite=Lax"
{"detail":"Successfully logged out."}
```

