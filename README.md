# docker-powerdns-dev

> A programmable DNS setup for your local development needs.

This Dockerfile prepares a PowerDNS 3.4-rc.1 server with the new [RESTful API](https://github.com/PowerDNS/pdnsapi) enabled.

## Quickstart

  docker run -p 1234:8081 -p 53/udp samcday/powerdns-dev

You can then start issuing REST calls on port 1234 to your Docker host.

## Use cases

When you want to run a reliable and powerful DNS server and have precise control over its responses.

For example, I'm using this to set up a functional testing environment for a MTA I'm working on. Thanks to stuff like SPF / DKIM / other sophisticated mailserver protocols, full control over DNS is very important.

## License

This project is released under the [MIT License](LICENSE)
