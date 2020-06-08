Project configuration files to integrate all the MyLife services in one docker-compose file for deployment.

## Context

The MyLife project involves several individual components that need to be combined in order for full solution to work.

The different components can be found as open source code under our [Gitlab](https://gitlab.com/my-life-ua) and [Github](https://github.com/my-life-ua) groups.

However, we have some built packages also available for download and use. The goal of this repository is to provide configuration files (mainly through [docker](https://www.docker.com/) and [docker-compose](https://docs.docker.com/compose/)) that would allow anyone to run it, and that are also the way we are able to deploy all the services to our deployment server (private to the University of Aveiro's network).

## Usage

You can start using this solution simply by:
```
docker-compose up [-d]
```
(assuming you have `docker` and `docker-compose` installed, and have some basic knowledge about these tools)

## Notes

We are able to use this repository for deploying our services thanks to the ability to trigger pipelines from one repository to another in Gitlab. That way, when there is a commit in an "upstream" repository, this deployment pipeline is automatically triggered.
