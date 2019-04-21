# Plex-docker

Simple project for fast deploy PLEX in docker container.

Official image page: https://github.com/plexinc/pms-docker

For deploy(with default timezone Europe/Moscow):
```sh
docker-compose up -d
mkdir -f src/data/movies
sudo chmod -R 777 src/data/movies
```

If you have a different time zone:
```sh
export TZ=Europe/London && docker-compose up -d
mkdir -f src/data/movies
sudo chmod -R 777 src/data/movies
```

Next, move your movies to the src/data/movies directory.