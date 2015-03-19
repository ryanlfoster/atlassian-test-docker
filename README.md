# atlassian-test-docker

## Prerequisites

- docker
- docker-compose

## Usage

- Add the following to your `/etc/hosts`

```
127.0.0.1   crowd.test.net
127.0.0.1   jira.test.net
127.0.0.1   stash.test.net
127.0.0.1   bamboo.test.net
127.0.0.1   confluence.test.net
```

- Run 

```
docker-compose up
```

- Finish configuration by connecting to
  - http://crowd.test.net/
  - http://jira.test.net/
  - http://stash.test.net/
  - http://bamboo.test.net/
  - http://confluence.test.net/
- Optionally configure with Postgres databases at
  - `postgres.test.net:5432`
  - Crowd
    - database `crowd`
    - user `crowd`
    - password `crowd`
  - CrowdID
    - database `crowdid`
    - user `crowd`
    - password `crowd`
  - JIRA
    - database `jira`
    - user `jira`
    - password `jira`
  - Stash
    - database `stash`
    - user `stash`
    - password `stash`
  - Bamboo
    - database `bamboo`
    - user `bamboo`
    - password `bamboo`
  - Confluence
    - database `confluence`
    - user `confluence`
    - password `confluence`

## Resetting data

- Run

```
docker-compose rm
```

## Deployment notes


