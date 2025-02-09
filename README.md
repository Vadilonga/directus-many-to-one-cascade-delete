# Directus Many To One Cascade Delete

This repository contains a docker-compose.yml file that can be used to run a Directus instance with the schema defined in schema.yml configured to cascade delete on the Many To One relationship.

## Requirements

- Docker
- Docker Compose

## Usage

1. Clone the repository
2. Run `docker-compose up`
3. Open your browser and go to http://localhost:8055
4. Create a new item named "A" in the `nodes` collection
5. Create a new item named "B" in the `nodes` collection ad set the node "A" as the parent
6. Create a new item named "C" in the `nodes` collection ad set the node "B" as the parent
7. Delete the node "A" and observe that the nodes "B" and "C" are also deleted

