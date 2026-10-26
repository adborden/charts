# charts

Helm charts from adborden.

- [wallabag](https://wallabag.org/) read-it-later service

## Usage

Add this helm repository.

    helm repo add adborden https://adborden.github.io/charts

Install a chart.

    helm install wallabag adborden/wallabag

## Development

Template your chart.

    helm template example charts/wallabag --debug

Lint your chart.

```bash
make lint
```

Create a kind cluster for chart-testing.

```bash
kind create cluster
```

Run the chart testing.

```bash
make test
```

## Release

Run all the checks.

```bash
make docs lint test
```

Bump the chart version if necessary.
