tutorial blog
link [building-and-testing-a-rest-api-in-go-with-gorilla-mux-and-postgresql](https://semaphoreci.com/community/tutorials/building-and-testing-a-rest-api-in-go-with-gorilla-mux-and-postgresql)

bring postgres up

```shell
docker run --name postgresql -e POSTGRES_USER=myusername -e POSTGRES_PASSWORD=mypassword -p 5432:5432 -v ~/data:/var/lib/postgresql/data -d postgres
```

export db creds:

```shell
export APP_DB_USERNAME=myusername
export APP_DB_PASSWORD=mypassword
export APP_DB_NAME=postgres
```

run `go test -v`

well done!

to direct login to db using psql:

```shell
docker run -it --rm jbergknoff/postgresql-client postgresql://myusername:mypassword@192.168.1.48:5432
```