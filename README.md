
tutorial blog link [building-and-testing-a-rest-api-in-go-with-gorilla-mux-and-postgresql](https://semaphoreci.com/community/tutorials/building-and-testing-a-rest-api-in-go-with-gorilla-mux-and-postgresql)

```
docker run --name postgresql -e POSTGRES_USER=myusername -e POSTGRES_PASSWORD=mypassword -p 5432:5432 -v ~/data:/var/lib/postgresql/data -d postgres
docker run -it --rm jbergknoff/postgresql-client postgresql://myusername:mypassword@192.168.1.48:5432
```