# Polkadot PRE | Running the Software
The following steps allow you to run the Polkscan PRE stack by using our prebuilt Docker containers.

## Run application with prebuilt Docker Hub images
Git clone
```bash
git clone https://github.com/polkascan/polkascan-pre.git
```

Change directory
```bash
cd polkascan-pre
```

Check tags/releases
```bash
git tag
```

Check tags/releases
```bash
git checkout [tag/release]
```

Checkout depending submodules
```bash
git submodule update --init --recursive
```

During the first run let MySQL initialize (wait for 30 seconds)
```bash
docker-compose up -d mysql
```

Then start the other docker containers
```bash
docker-compose up
```

## Links
* Polkascan Explorer GUI: http://127.0.0.1:8080
* Harvester task monitor: http://127.0.0.1:5555
* Harvester progress: http://127.0.0.1:8080/harvester/admin
