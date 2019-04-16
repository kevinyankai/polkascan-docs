# Polkadot PRE | Software Architecture

## 1. Primary Applications
### 1.1. Polkascan PRE Harvester
The Polkascan PRE Harvester Application transforms a Substrate node's raw data into relational data for various classes of objects, such as: blocks, runtime metadata entities, extrinsics, events and various runtime data entities, such as: timestamps, accounts and balances. [Repository](https://github.com/polkascan/polkascan-pre-harvester)

### 1.2. Polkascan PRE Explorer API
The Polkascan PRE Explorer API Application makes the data which is produced by the Polkascan PRE Harvester Application accessible to developers by providing JSON-API data on RESTful endpoint. The Polkascan PRE Explorer API Application will provide endpoints to all harvested data. [Repository](https://github.com/polkascan/polkascan-pre-explorer-api)

### 1.3. Polkascan PRE Explorer GUI
The purpose of the Polkascan PRE Explorer GUI Application is to make the data which is produced by the Polkascan PRE Harvester Application and disseminated by the Polkascan PRE Explorer API Application accessible to day-to-day end-user. The Polkascan PRE Explorer GUI Application provides a user interface to the Polkascan PRE Explorer API Application and intends to showcase what developers should be able to build on top of the Polkascan PRE Explorer API Application for a wide audience of day-to-day users. [Repository](https://github.com/polkascan/polkascan-pre-explorer-gui)

## 2. Libraries
### 2.1. Python Substrate Interface Library
This library specializes in interfacing with a Substrate node. [Repository](https://github.com/polkascan/py-substrate-interface)

### 2.2. Python SCALE Codec Library
Most of the data that the Substrate RPCs output is encoded with the SCALE Codec. This codec is used by the Substrate nodes' internal runtime. In order to get to meaningful data?this data will need to be decoded. The Python SCALE Codec Library will specialize in this task. [Repository](https://github.com/polkascan/py-scale-codec)

## 3. Docker Compose
### 3.1. Polkascan PRE Docker Compose 
Docker Compose files to run and/or build the entire Polkascan PRE Application stack. [Repository](https://github.com/polkascan/polkascan-pre)

### 3.2. Various Dockerfiles
All referenced repositories have a Dockerfile in the project root that enables building the application from source.

## 4. Prebuilt Components 
### 4.1. Polkascan @ Docker Hub
* [Polkascan PRE Harvester](https://hub.docker.com/r/polkascan/pre-harvester)
* [Polkascan PRE Explorer API](https://hub.docker.com/r/polkascan/pre-explorer-api)
* [Polkascan PRE Explorer GUI](https://hub.docker.com/r/polkascan/pre-explorer-gui)

### 4.2. Polkasource @ Docker Hub
* [Polkasource Substrate Node for Alexander Network](https://hub.docker.com/r/polkasource/substrate-alexander)
* [Polkasource Substrate Node for Edgeware Network](https://hub.docker.com/r/polkasource/substrate-edgeware)
* [Polkasource Substrate Node for Robonomics Network](https://hub.docker.com/r/polkasource/substrate-robonomics)

### 4.3. Other Components @ Docker Hub
* [MySQL](https://hub.docker.com/_/mysql)
* [Redis](https://hub.docker.com/_/redis)
* [Nginx](https://hub.docker.com/_/nginx)
