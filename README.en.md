# Yandex Market Notification service API Integration Guide for Sellers

This guide explains how to use the Yandex Market Notification service API specification for sellers, designed to automate and streamline interactions with the marketplace.

## Generating a Notification service API Client

The specification helps generate server files in any language or framework supported by the OpenAPI generator. This can significantly simplify integration with Yandex Market via the Notification service API.

### Obtaining the Specification via Git

Choose one of these two methods:
1. Clone the repository by executing the following command: `git clone https://github.com/yandex-market/yandex-market-notification-api.git`.
2. Download the archive from the repository using the GitHub web interface: click the green `Code` button and select `Download ZIP` from the dropdown menu.

### Installing the OpenAPI Generator via Package Managers

Refer to the generator documentation: <https://openapi-generator.tech/docs/installation>

**Using npm (any OS)**
`npm install @openapitools/openapi-generator-cli -g`

**Using Homebrew (macOS)**
`brew install openapi-generator`

**Using Scoop (Windows)**
`scoop install openapi-generator-cli`

### Generating the Server (contracts/models)

**Using npm (any OS)**
`npx @openapitools/openapi-generator-cli generate -i <path to openapi.yaml> -g <generator> -o <output path>`

**Using other package managers**
`openapi-generator generate -i <path to openapi.yaml> -g <generator> -o <output path> `

Explanation of placeholders:

* `<generator>` means the generator parameter for the chosen language or framework.
* `<output path>` means the directory where the generated server code will be saved.
* `<path to openapi.yaml>` means the path to the openapi.yaml file of this specification.

Examples of available generators include:
* spring
* kotlin-spring
* go-server
* aspnetcore
* python-flask
* nodejs-express-server

For a complete list of generators, visit: <https://openapi-generator.tech/docs/generators>
