# neo4j-node-friend-cli

This is a CLI app to experiment with neo4j. This app allows you to add people and befriend them. This is a port of the [neo4j-friends-cli](https://github.com/mdbottino/neo4j-friends-cli) Python app.

## Overview

The goal is to use a very simple data model to experiment with Cypher and neo4j. Using a (sort of) realistic dataset shows the strenghts and weakneses of the database. It's also a great way to get the hands dirty and see what you can acomplish using Cypher. This little app solves the classic "list friends of a friend" problem.

## Installation

You can install the dependencies using the provided `package.json` and `package-lock.json` files:

> npm install

The suggested node version is 14 as at the time of this writing is the LTS version available.

## Running the script

> node index.js

Commands that will be available:

- add (Add a person to the graph)
- befriend (Make two existing persons friends)
- edit (Update the age of a certain person)
- info (Get a summary of the nodes and relationships in the graph)
- list (Get the friends of a person)
- remove (Delete a person and all it's relationships from the graph)

## Data model

In the folder **docs** there is a file named **data-model.png** with an example of the data model. There is only one node label (Person) and one relationship type (FRIENDS_OF).
