# NodeRedPowerComboIntegration
Node-Red flow to switch KAT500 tuner mode and antenna and KPA500 band based on N1MM UDP data

## Docker commands to create container:

docker network create iot

docker volume create node_red_data

docker run -d -p 1880:1880 -p 12333:12333/udp --network iot -v node_red_data:/data --name nrcontrol nodered/node-red


## Within node-red, install:
node-red-dashboard

node-red-contrib-startup-trigger
