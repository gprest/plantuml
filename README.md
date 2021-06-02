# plantuml
A self-contained PlantUML workspace.

## PlantUML Server installation journal
- Searched on Google for `dockerhub plantuml`
- First result: https://hub.docker.com/r/plantuml/plantuml-server
- On that page, found a Docker launch command:

```docker run -d -p 8080:8080 plantuml/plantuml-server:jetty```

- Retrieved the composer equivalent (https://www.composerize.com/) and updated `docker-compose.yml`
- Mapped the server to port `18080` and exposed it outside the container
- Rebuilt the container and validated the server was up at http://localhost:18080
