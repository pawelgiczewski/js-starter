# js-starter
Starter template for containerized web project 

- frontend framework -> Vue.js
- backend framework -> Nest.js

## Docker compose for local development

apps served:
```
frontend -> http://localhost:30000
backend -> http://localhost:30000/api/v1
```

### Test | Demo
- Containers contains built app
- Containers may be used for cluster deployment 
- Want to see changes? Rebuild!
```
docker-compose up --build
```


### Development
- Apps served in watch mode - code changes are immediately reflected in app
```
./run-dev
```

## Adding new app/container checklist:
Update:
- docker-compose.yml
- docker-compose.watch.override.yml
- dev-tools/compose-reverse-proxy/conf.d/default.conf

Provide if needed:
- Dockerfile
- Dockerfile-watch
