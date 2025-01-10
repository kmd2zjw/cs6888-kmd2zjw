You must have [Docker](https://www.docker.com/get-started) and [Docker Compose](https://docs.docker.com/compose/install/) installed.

```
git clone git@github.com:matthewbdwyer/cs6888-Spring2025.git
cd cs6888-public


docker-compose up --build &
docker-compose exec main bash

build on x86 mac and publish at docker hub

check out whether you can build an apptainer sif from that docker image
e.g., https://rcs.ucalgary.ca/How_to_convert_a_Docker_container_to_an_Apptainer_container

and then execute it on portal.

This will allow people to run locally on their own machines or use portal.
I'm hoping it sidesteps the lack of docker-compose

apptainer build main.sif Apptainer.def &
apptainer exec main.sif bash

```
