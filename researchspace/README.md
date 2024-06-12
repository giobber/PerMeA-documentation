# ResearchSpace

## Links and documentation
- Main site: https://researchspace.org/
- GitHub (project): https://github.com/researchspace/researchspace
- GitHub (docker-compose): https://github.com/researchspace/researchspace-docker-compose
- GitHub (ontologies): https://github.com/researchspace/researchspace-instance-configurations

## How to install
### Docker
```shell
$ git clone git@github.com:researchspace/researchspace-docker-compose.git
$ cd researchspace-docker-compose/
$ cd basic/
```

Edit `.env` file: 
- Change `COMPOSE_PROJECT_NAME` to a proper prefix for docker containers
- **IMPORTANT**: Increase `BLAZEGRAPH_MEMORY` (4g value works for me on 2024/06/12)

```shell
$ docker compose up -d
```

To check logs
```shell
$ docker compose logs
$ docker compose logs <container>
```

