<br />
<p align="center">
  <a href="https://github.com/otasoft/otasoft-proxy">
    <img src="doc/otasoft-proxy-logo.png" alt="Otasoft Logo" width="128" height="128">
  </a>

  <h1 align="center">Otasoft Proxy - Proxy and Firewall service for OTA API Gateway</h1>

  <p align="center">
    <a href="https://github.com/otasoft/otasoft-core/issues">Report Bug</a>
    ·
    <a href="https://github.com/otasoft/otasoft-core/issues">Request Feature</a>
  </p>
</p>

## About The Project
Otasoft Proxy is a proxy and firewall service for API Gateway in Online Travel Agency Ecosystem. It rejects unwanted requests and transfer correct ones to the API Gateway. It guarantees network layer security between client applications and the API Gateway

* Nginx
* Haproxy
* iptables (firewalld)
* Docker

Otasoft projects are and always will be open source (MIT Licence). Anyone can use and support the project. The project is currently in the development phase.

## Table of Contents

* [Getting Started](#getting-started)
* [Usage](#usage)
* [Roadmap](#roadmap)
* [Contributing](#contributing)
* [How to support?](#how-to-support?)
* [Contact](#contact)
* [License](#license)

<!-- GETTING STARTED -->
## Getting Started

To start developing the project please check if you have these tools installed on your machine:

* [Node.js](https://nodejs.org/en/download/)
* [Yarn](https://yarnpkg.com/getting-started/install)
* [Docker](https://www.docker.com/get-started)

Installation

1. Clone the repo
```sh
git clone https://github.com/otasoft/otasoft-proxy
```
3. Copy .env.example file as .env and fill it with your environment variables
```sh
cp .env.example .env # Linux and Mac

copy .env.example .env # Windows
```
4. Run script to generate OpenSSL public certificate and private key
```sh
sh /scripts/generate-nginx-ssl-cert.sh # Linux and Mac

bash /scripts/generate-nginx-ssl-cert.sh # Windows

# If you dont have bash installed this link could help you 
# https://stackoverflow.com/questions/26522789/how-to-run-sh-on-windows-command-prompt
```
5. Add static entry in etc/hosts for otasoft-proxy
```sh
sudo nano /etc/hosts # Linux and Mac

edit C:\Windows\System32\drivers\etc\hosts # Windows

> 127.0.0.1 proxy.otasoft.org
```
6. Run docker-compose to start the proxy service
```sh
docker-compose up
```

<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/otasoft/otasoft-core/issues) for a list of proposed features (and known issues).

<!-- CONTRIBUTING -->
## Contributing

You are welcome to contribute to Otasoft projects. Please see [contribution tips](CONTRIBUTING.md)

<!-- SUPPORT -->
## How to support?
Otasoft projects are and always will be Open Source.

Core team and contributors in the Otasoft ecosystem spend their free and off work time to make this project grow. If you would like to support us you can do so by:

- contributing - it does not matter whether it is writing code, creating designs, or sharing knowledge in our e-books and pdfs. Any help is always welcome! 
- evangelizing - share a good news about Otasoft projects in social media or during technology conferences ;)

<!-- CONTACT -->
## Contact

Founder -> [Jakub Andrzejewski](https://www.linkedin.com/in/jakub-andrzejewski/)

<!-- LICENSE -->
## License

Distributed under the [MIT licensed](LICENSE). See `LICENSE` for more information.