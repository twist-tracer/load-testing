# Load testing repo

## Usage

1. Copy load.example.yaml to load.yaml and setup
```bash
cp load.example.yaml load.yaml
```

2. Run tests in docker
```bash
docker-compose up
```

## Overload usage

1. Register on https://overload.yandex.net and copy api token
2. Create token.txt file and paster token there

3. Paste this to load.yaml config
```yaml
overload:
  enabled: true
  package: yandextank.plugins.DataUploader
  token_file: token.txt
```
