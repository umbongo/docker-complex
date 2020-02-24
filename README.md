# docker-complex
test site - docker multicontainer / microservices.

uses: 
- docker container for each service
- react - frontend
- express.js - API layer
- redis - var Store
- worker - app layer
- postgres - data store.

topology:
user ---> react --> express.js --> redis <--> worker
                        |
                        | <--> postgres


