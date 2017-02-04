# Debian Jessie Docker

Packer templates to build a Docker Debian Jessie base image.

## Synopsis

This script will create a Docker base image with a minimum installation of
Debian Jessie.

This script creates what is called a *Base Image* for Docker from scratch
using technology other than Docker for that.

## Getting Started

There are a couple of things needed for the templates to work.

### Prerequisites

Packer tools need to be installed on your local computer.

#### Packer

Packer installation instructions can be found [here](https://www.packer.io/docs/installation.html).

#### Virtualbox

Virtualbox installation instructions can be found [here](https://www.virtualbox.org/wiki/Downloads).

### Installation

Nothing special to be done. Just download the template that you wish to use.

### Usage

In order to create the base image using this packer script you may have to
provide a few options.

```
Usage:
  packer build [-var 'option=value'] jessie.json
```

#### Script Options
- `docker_name` - The Docker image name (default value: "jessie").
- `headless` - Show the console of the machine being built (default value: "true").
- `os_codename` - Codename of Operating System (default value: "jessie").
- `os_version` - Version of the Operating System (default value: "8.7.1").

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## Versioning

This project uses [SemVer](http://semver.org/) for versioning. For the versions
available, see the [tags on this repository](https://github.com/fscm/packer-docker-debian/tags).

## Authors

* **Frederico Martins** - [fscm](https://github.com/fscm)

See also the list of [contributors](https://github.com/fscm/packer-docker-debian/contributors)
who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE](../LICENSE)
file for details
