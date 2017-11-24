# image-search-abstraction-layer
Freecodecamp's API Project for Back End Development Certification

User Stories:

- I can get the image URLs, alt text and page urls for a set of images relating to a given search string.
- I can paginate through the responses by adding a ?offset=2 parameter to the URL.
- I can get a list of the most recently submitted search strings.

## Requirements
* Docker
* Create a Google Custom Search Engine: https://cse.google.com/cse

## Installation
* `docker-compose build` - to build mongodb and node services

## Usage
* `docker-compose up` - to start the services

* `docker-compose down` - to stop the services

## Example Usage

Get the port of your app that Docker mapped on your machine.

`http://localhost:3000/api/imagesearch/lolcats funny?offset=10` - to search

`https://localhost:3000/api/latest/imagesearch/` - to list the latest searches

## Example Output

`[{"term":"lolcat","when":"2017-11-23T21:40:28.111Z"},{"term":"minecraft","when":"2017-11-23T21:28:13.399Z"}]` - latest searches
