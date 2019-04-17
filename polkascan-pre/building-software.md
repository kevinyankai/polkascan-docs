# Polkadot PRE | Building the Software
The following steps allow you to run the Polkscan PRE stack by building the software from the various source repositories.

## Run application and build from source
Git clone
```bash
https://github.com/polkascan/polkascan-pre.git
```

Change directory
```bash
cd polkascan-pre
```

Make sure to also clone submodules within the cloned directory: 
```bash
git submodule update --init --recursive
```

Check tags/releases
```bash
git tag
```

Check tags/releases
```bash
git checkout [tag/release]
```

During the first run let MySQL initialize (wait for 30 seconds)
```bash
docker-compose -f docker-compose.dev.yml up -d mysql
```

Then build the other docker containers
```bash
docker-compose -f docker-compose.dev.yml up --build
```

## Links
* Polkascan Explorer GUI: http://127.0.0.1:8080
* Harvester task monitor: http://127.0.0.1:5555
* Harvester progress: http://127.0.0.1:8080/harvester/admin
