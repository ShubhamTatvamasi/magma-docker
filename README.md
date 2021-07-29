# magma-docker

clone magma repo:
```bash
git clone https://github.com/magma/magma.git
```

move to docker folder and build Orchestrator images:
```bash
cd magma/orc8r/cloud/docker
./build.py --all
```

start Orchestrator:
```bash
./run.py --metrics
```

move to NMS folder:
```bash
cd magma/nms/app/packages/magmalte
docker-compose build magmalte
docker-compose up -d
./scripts/dev_setup.sh
```

https://magma-test.localhost/
```
ID: admin@magma.test
Password: password1234
```
