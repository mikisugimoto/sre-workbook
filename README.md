# SRE-workbook

Learning how to do SRE stuff!

## Modules

Each module is a small task representing a skill or technology

### Containerize an Application

**Objective**: Run a .NET API in Docker

**Definition of Done**:
- [ ] Create a Dockerfile which copies in the application files, compiles the application, and runs on container start
- [ ] Update the `./service/README.md` so users know how to build and run the Docker container locally and hit the endpoints

**Resources**:
- [Docker architecture](https://docs.docker.com/get-started/overview/#docker-architecture)
- [Dockerfile reference](https://docs.docker.com/engine/reference/builder/)
- [Dockerfile best practices](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/)
- [Microsoft .NET Docker Hub repository](https://hub.docker.com/_/microsoft-dotnet/)

**Hints**:
* The HTTP port is `80`, the HTTPS port is `443`

