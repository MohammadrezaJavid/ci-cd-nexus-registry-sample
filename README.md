# Docker private registry

In this repository, I implement a private docker registry and a docker proxy to speed up the CI/CD workflow.

In this scenario, only two ports 80 and 443 of the server are open.
We receive all the requests from two ports(80 & 443), then separate the requests using traefik as a reverse proxy.

We implement two services, traefik and nexus, using containers.

## Traefik

UI traefik, [traefik.localhost](https://traefik.localhost/) ----> port: 8080

## Nexus

UI nexus, [registry.localhost](https://registry.localhost/) ----> 8081

Docker proxy, [docker.localhost](https://docker.localhost/) ----> 8082

Docker private registry, [private.localhost](https://private.localhost/) ----> 8083

#

The general scenario of the repo is drawn in this file: ![general structure](./images/general-structure.pdf)

# Setup docker private registry

TODO

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
