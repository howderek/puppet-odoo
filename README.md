# odoo9

#### Table of Contents

1. [Description](#description)
1. [Setup - The basics of getting started with odoo9](#setup)
    * [What odoo9 affects](#what-odoo9-affects)
    * [Beginning with odoo9](#beginning-with-odoo9)
1. [Usage - Configuration options and additional functionality](#usage)
1. [Reference - An under-the-hood peek at what the module is doing and how](#reference)
1. [Limitations - OS compatibility, etc.](#limitations)
1. [Development - Guide for contributing to the module](#development)

## Description

Install Odoo 9 Communinty edition in a manner similar to that described in
*[Installing Odoo](https://www.odoo.com/documentation/9.0/setup/install.html)*.

## Setup

### What odoo9 affects

* Installs the `odoo` package from the Odoo repository.
* Configures `/etc/odoo/openerp-server.conf`.
* Manipulates the running state of the `odoo` service.
* Optionally configures repositories to enable package installations from
  the Odoo nightly builds.
* Optionally installs the `wkhtmltopdf` package from the Odoo repository.

### Beginning with odoo9

```puppet
include ::odoo9
```

## Usage

This section is where you describe how to customize, configure, and do the
fancy stuff with your module here. It's especially helpful if you include usage
examples and code samples for doing things with your module.

## Reference

### Attributes

#### Class odoo9

##### `install_wkhtmltopdf`
Whether or not to install the optional `wkhtmltopdf` package from the Odoo
repository.
Default value **false**.

## Limitations

At the moment this module has only been tested against Ubuntu 14.

## Development

Contributions will be gratefully accepted. Please go to the project page, fork
the project, make your changes locally and then raise a pull request. Details
on how to do this are available at
https://guides.github.com/activities/contributing-to-open-source.
