# docker-complex
test site - docker multicontainer / microservices.

uses: 
- docker container for each service
- nginx - webserver
- react - web frontend
- express.js - API server
- redis - dict store
- postgres - permanent data store
- worker - application logic


topology:
nginx   ---> react 
        ---> express.js 
                <--> postgres
                --> redis <--> worker
                        


