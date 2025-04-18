# Docker Registry Browser

Web Interface for the [Docker Registry HTTP API V2](https://distribution.github.io/distribution/spec/api/) written in Ruby on Rails.

## Screenshots

Repositories overview

[![Screenshot 1](https://github.com/klausmeyer/docker-registry-browser/raw/master/docs/screenshot1_thumb.png "Screenshot 1")](https://github.com/klausmeyer/docker-registry-browser/raw/master/docs/screenshot1.png)

Tag overview

[![Screenshot 2](https://github.com/klausmeyer/docker-registry-browser/raw/master/docs/screenshot2_thumb.png "Screenshot 2")](https://github.com/klausmeyer/docker-registry-browser/raw/master/docs/screenshot2.png)

Tag details

[![Screenshot 3](https://github.com/klausmeyer/docker-registry-browser/raw/master/docs/screenshot3_thumb.png "Screenshot 3")](https://github.com/klausmeyer/docker-registry-browser/raw/master/docs/screenshot3.png)

Delete tag

[![Screenshot 4](https://github.com/klausmeyer/docker-registry-browser/raw/master/docs/screenshot4_thumb.png "Screenshot 4")](https://github.com/klausmeyer/docker-registry-browser/raw/master/docs/screenshot4.png)

## Usage

Please have a look at the [Documentation](https://github.com/klausmeyer/docker-registry-browser/blob/master/docs/README.md) for more details and available configuration options.

### Docker

```shell
$ docker run --name registry-browser -e SECRET_KEY_BASE=changeme -p 8080:8080 klausmeyer/docker-registry-browser
```

Note: The value for `SECRET_KEY_BASE` can be generated via `openssl rand -hex 64`

### Kubernetes (Helm)

A helm-chart is available at [klausmeyer/helm-charts](https://github.com/klausmeyer/helm-charts/tree/master/charts/docker-registry-browser).

## Licence

The application is available as open source under the terms of the MIT License.
