# KrakenD-contrib

A list of awesome modules and adaptors for the [KrakenD](https://github.com/devopsfaith/krakend) framework.

## Encoding

1. [krakend-xml](https://github.com/devopsfaith/krakend-xml)
2. [krakend-rss](https://github.com/devopsfaith/krakend-rss)

## Circuit Breaker

1. [gobreaker](https://github.com/devopsfaith/krakend-circuitbreaker/tree/master/gobreaker) contains an adaptor over the github.com/sony/gobreaker lib
2. [eapache](https://github.com/devopsfaith/krakend-circuitbreaker/tree/master/eapache) is a simple proxy adaptor for the github.com/eapache/go-resiliency/breaker circuit breaker implementation

## Rate-limit

1. [rate](https://github.com/devopsfaith/krakend-ratelimit/tree/master/rate) embeds the golang.org/x/time/rate token bucket implementation into the proxy and router layers
2. [juju](https://github.com/devopsfaith/krakend-ratelimit/tree/master/juju) implements a rate limiter proxy and router using the github.com/juju/ratelimit lib

## Request and response manipulation

1. [krakend-martian](https://github.com/devopsfaith/krakend-martian) injects martian modifiers into the KrakenD proxy pipe

## Security

### OAuth2 client credentials

1. [krakend-oauth2-clientcredentialst](https://github.com/devopsfaith/krakend-oauth2-clientcredentials) offers a proxy.HTTPClientFactory implementation wrapping the golang.org/x/oauth2/clientcredentials lib
