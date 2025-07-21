# hydroserver-1.2
Easy Local Deployment with Podman 

### simple setup and start script

cli command: 

`
. start.sh
`

### Setup

`
podman compose -f setup-compose.yaml up
`

### Run Podman

`
podman compose up
`

### After container startup

**go to:**

**frontend nginx:**

- http://localhost:3030/Login

**test frontend:**

- http://localhost:5173/login?next=/sites

**django admin:**

- http://localhost:8000/admin/