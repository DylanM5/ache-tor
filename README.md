# ACHE-Tor Dark Web Crawler

An [ACHE](https://github.com/VIDA-NYU/ache) implementation to discover and index `.onion` sites. Part of a research project at Virginia Tech.

# TODO
- Literature review
- Get running on server
- Fetch only .onion, homepages, and pages that have account creation capabilities 
    - SMILE model or DB queries?
- Migrate to GitLab
- Figure out how often it will run
- Should we add documenting change over time

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/)

## Getting Started

**Start the crawler:**
```bash
docker-compose up -d
```

**Stop the crawler:**
```bash
docker-compose down
```

**View logs:**
```bash
docker-compose logs -f ache
```

## Web Interfaces

| Service       | URL                     |
|---------------|-------------------------|
| ACHE Dashboard| http://localhost:8080   |
| Elasticsearch | http://localhost:9200   |

## Adding Seed URLs
Edit `tor.seeds` and add one `.onion` URL per line