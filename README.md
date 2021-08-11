# meilisearch

## Recommended system requirements

- A linux box or VM (eg: Ubuntu)
- 2 cores of CPU
- 2 to 4 Gb of RAM space

## Prerequisite

- [Docker](https://docs.docker.com/engine/install/)
- [docker-compose](https://docs.docker.com/compose/install/)

## Environment 

Set ``MEILI_MASTER_KEY`` environment variable to allow only applications with the Key API.

Set ``MEILISEARCH_HOST_URL`` environment variable to set meilisearch url instance to use scraper

## Usage

```bash
mkdir meilisearch/
cd meilisearch/

wget --no-check-certificate https://raw.githubusercontent.com/ezpaarse-project/meilisearch/master/docker-compose.yml

docker-compose up -d
```

## Scrapers

Create a [GitHub Action](https://github.com/meilisearch/docs-scraper#in-a-github-action-) in your repository that contains your documentation.

Add your scraper JSON file in the same repository, edit it to change the value of ``start_urls``.

Examples :
- [VuePress](https://github.cm/ezpaarse-project/meilisearch/master/scrapers/vuepress.json)
