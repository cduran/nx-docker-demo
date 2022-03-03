

# Nx and Docker demo

This project was generated using [Nx](https://nx.dev).


## To run this demo
```bash
npx nx run-many --target=serve --projects=api,html --parallel
```

## To build docker images
```bash
npx nx run-many --target=build --projects=api,html --parallel
```
> FYI, we use internally this docker commands:
> 
> `docker build -f ./apps/api/Dockerfile . -t api`
> 
> `docker build -f ./apps/html/Dockerfile . -t html`

## If modifications are made to any project
```bash
npx nx deploy html
```
or
```bash
npx nx deploy api
```

## Finally to run with docker compose
```bash
docker compose up
```
