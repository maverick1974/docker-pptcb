# docker-pptcb

This container is a poc developed for PuppetConf 2016 in order to download and extract puppet codebase artifacts within a container that will present its volumes to a puppetserver one

## Usage

### Build

```
docker build -t mvisonneau/pptcb .
```

### Run

```
docker run -d -e URL=https://gitlab.example.com -e PROJECT=<your_project_id> -e TOKEN=<your_api_token> --name pptcb <yourname>/pptcb
```

## Prerequisites

- Works with Gitlab > 8.2
- Assume that you have .deb files being made by your CI processes, exposed as artifacts and that contains puppet code
