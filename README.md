# hydroserver-1.2

Easy Local Deployment with Podman  with simple setup and start script

cli command: 

`. start.sh`

**Setup**

`podman compose -f setup-compose.yaml up`

**Run Podman**

`podman compose up`

**After container startup go to:**

frontend nginx:

- http://localhost:3030/Login

test frontend:

- http://localhost:5173/login?next=/sites

django admin:

- http://localhost:8000/admin/

## Debugger

debugpy with vscode launch.json

usage: 

change in `docker-compose.yaml`

`standardcommand` to `debugcommand`

then type in cli:

`podman compose up` 

click start `launch.json` from vscode

## Bugs

dependency error [pool-1] from deprecated moduls:

`
hsclient -> hsmodels -> rdflib must be lower than version 6.0.0 
`