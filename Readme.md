## Graphite and grafana containers
The docker container for grahite and grafana. There following three volumes mapped: 
- `./data/whisper` to `/opt/graphite/storage/whisper`
- `./data/grafana` to `/opt/grafana/data`
- `./log/graphite` to `/opt/graphite/storage/log`

### Expose ports for Graphite
- 2003 
- 81 (Web UI). `http://localhost:81` is the web for grahite

### Expose ports for Grafana
- 80 (Web UI) `http://localhost` is the web for grafana. The username and password is 'admin:admin' 

### Build the container 
`docker-compose build`
### Run the container
`docker-compose up -d`

