# Perf Testing

## Pre-requisites
- Install Taurus: https://gettaurus.org/docs/Installation/

## Run tests
- bzt `<filename>`.yml
- Artifacts: /`%Y-%m-%d_%H-%M-%S.%f`

## Run in docker
- docker run -v $(pwd):/bzt-configs -v $(pwd)/reports:/tmp/artifacts blazemeter/taurus tests/`<filename>`.yml
$(pwd) = "Print Working Directory"
- Artifacts: /reports
