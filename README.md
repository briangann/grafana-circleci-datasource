# Grafana Data Source for CircleCI

[![CircleCI](https://circleci.com/gh/briangann/grafana-circleci-datasource/tree/master.svg?style=shield)](https://circleci.com/gh/briangann/grafana-circleci-datasource/tree/master)
[![David Dependency Status](https://david-dm.org/briangann/grafana-circleci-datasource.svg)](https://david-dm.org/briangann/grafana-circleci-datasource)
[![David Dev Dependency Status](https://david-dm.org/briangann/grafana-circleci-datasource/dev-status.svg)](https://david-dm.org/briangann/grafana-circleci-datasource/?type=dev)
[![Known Vulnerabilities](https://snyk.io/test/github/briangann/grafana-circleci-datasource/badge.svg)](https://snyk.io/test/github/briangann/grafana-circleci-datasource)

[![Maintainability](https://api.codeclimate.com/v1/badges/e9c4cd2714cba0fdae56/maintainability)](https://codeclimate.com/github/briangann/grafana-circleci-datasource/maintainability)
[![Test Coverage](https://api.codeclimate.com/v1/badges/e9c4cd2714cba0fdae56/test_coverage)](https://codeclimate.com/github/briangann/grafana-circleci-datasource/test_coverage)

## Docker Support

A docker-compose.yml file is include for easy development and testing, just run

```BASH
docker-compose up
```

Then browse to <http://localhost:3000>

## External Dependencies

* Grafana 7.x

## Getting started

A data source backend plugin consists of both frontend and backend components.

### Frontend

1. Install dependencies

```BASH
yarn install
```

2. Build plugin in development mode or run in watch mode
```BASH
yarn dev
```
or
```BASH
yarn watch
```
3. Build plugin in production mode
```BASH
yarn build
```

### Backend

1. Update [Grafana plugin SDK for Go](https://grafana.com/docs/grafana/latest/developers/plugins/backend/grafana-plugin-sdk-for-go/) dependency to the latest minor version:

```bash
go get -u github.com/grafana/grafana-plugin-sdk-go
```

2. Build backend plugin binaries for Linux, Windows and Darwin:
```BASH
mage -v
```

3. List all available Mage targets for additional commands:
```BASH
mage -l
```

## Learn more

- [Build a data source backend plugin tutorial](https://grafana.com/tutorials/build-a-data-source-backend-plugin)
- [Grafana documentation](https://grafana.com/docs/)
- [Grafana Tutorials](https://grafana.com/tutorials/) - Grafana Tutorials are step-by-step guides that help you make the most of Grafana
- [Grafana UI Library](https://developers.grafana.com/ui) - UI components to help you build interfaces using Grafana Design System
- [Grafana plugin SDK for Go](https://grafana.com/docs/grafana/latest/developers/plugins/backend/grafana-plugin-sdk-for-go/)
