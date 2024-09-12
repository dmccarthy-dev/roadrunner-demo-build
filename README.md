# rr demo build process

Install the vx build tool
```
go install github.com/roadrunner-server/velox/v2024/cmd/vx@latest
```

Roadrunner Template

## Setup

Add GitHub token to path
```bash
export GH_REPOS_TOKEN=""
```

## Build
```bash
vx build -c plugins.toml
```

Linux Build 
```bash
GOOS=linux GOARCH=amd64 vx build -c roadrunner/plugins.toml 
```

## Deploy

```bash
cp rr ../roadrunner-demo-php/demo-setup-basic
cp rr ../roadrunner-demo-php/demo-setup-fiber
cp rr ../roadrunner-demo-php/demo-setup-middleware
cp rr ../roadrunner-demo-php/demo-setup-plugin
cp rr ../roadrunner-demo-php/demo-setup-basic-with-rpc
```