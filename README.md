# Cadence get started project

### Prerequisites
- Docker
- golang

### To run cadence server 
```bash
docker-compose up
```

### To run cadence worker
```bash
go run .
```
  

### To test cadence workflow

```bash
docker run --network=host --rm ubercadence/cli:master --domain test-domain workflow start --et 60 --tl test-worker --workflow_type main.helloWorldWorkflow --input '"This is another example"'
```
