# otel-collector

My personal OTel Collector Setup and Configuration to better mirror a professional environment from local

## Service Providers

- [Honeycomb](https://honeycomb.io)

I considered setting up a local stack with Grafana, Jaeger, Zipkin, Prometheus and other components to run this locally, but I find that I really enjoy working with Honeycomb.io for my personal stuff. So I'm going to configure all of the data to flow to honeycomb.

## Setup

For the moment, I'm using docker compose with local port bindings to setup an OTel Collector locally and forward my observability data.

### Docker Compose

I built this using Docker Compose for ease of use and portability across machines.

1. Run `cp .env.example .env` the first time
1. Edit the .env file with your personal access tokens
1. Run `docker compose up`
