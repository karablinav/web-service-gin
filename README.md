RESTful API with Go and Gin

Run application:
```bash
go run .
```

GET all albums:
```bash
curl http://localhost:8080/albums

curl http://localhost:8080/albums \
    --header "Content-Type: application/json" \
    --request "GET"
```

GET special album:
```bash
curl http://localhost:8080/albums/2
```

POST new album:
```bash
curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
```

