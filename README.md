# KrakenD-contrib

A list of awesome modules and adaptors for the [KrakenD](https://github.com/devopsfaith/krakend) framework.

## Metrics and instrumentation

1. [krakend-opencensus](https://github.com/devopsfaith/krakend-opencensus) simple opencensus adapter (InfluxDB,Zipkin,Prometheus,Jaeger,Logger)
2. [krakend-metrics](https://github.com/devopsfaith/krakend-metrics) contains a set of middlewares for the [KrakenD](https://github.com/devopsfaith/krakend) framework for instrumenting different parts of the pipes.
3. [letgoapp/krakend-influx](https://github.com/letgoapp/krakend-influx) adapter to send KrakenD metrics to an influxdb backend.
4. [krakend-newrelic](https://github.com/devopsfaith/krakend-newrelic) integrates the NewRelic agent at router, proxies and backend levels

## Encoding

1. [krakend-xml](https://github.com/devopsfaith/krakend-xml)
2. [krakend-rss](https://github.com/devopsfaith/krakend-rss)

## Service Discovery

1. [krakend-etcd](https://github.com/devopsfaith/krakend-etcd) is an etcd client and subscriber for the KrakenD framework.
2. [joaoqalves/krakend-eureka](https://github.com/joaoqalves/krakend-eureka) is an eureka client and subscriber for the KrakenD framework.
3. [krakend-consul](https://github.com/devopsfaith/krakend-consul) is a consul client for the KrakenD framework.
4. [schibsted/krakend-eureka](https://github.com/schibsted/krakend-eureka) is an eureka client and subscriber for the KrakenD framework.

## Circuit Breaker

1. [gobreaker](https://github.com/devopsfaith/krakend-circuitbreaker/tree/master/gobreaker) contains an adaptor over the github.com/sony/gobreaker lib
2. [eapache](https://github.com/devopsfaith/krakend-circuitbreaker/tree/master/eapache) is a simple proxy adaptor for the github.com/eapache/go-resiliency/breaker circuit breaker implementation
3. [hystrix](https://github.com/schibsted/krakend-cbreaker) cirbuit breaker implementation based on github.com/afex/hystrix-go

## Rate-limit

1. [rate](https://github.com/devopsfaith/krakend-ratelimit/tree/master/rate) embeds the golang.org/x/time/rate token bucket implementation into the proxy and router layers
2. [juju](https://github.com/devopsfaith/krakend-ratelimit/tree/master/juju) implements a rate limiter proxy and router using the github.com/juju/ratelimit lib
3. [schibsted/krakend-ratelimit](https://github.com/schibsted/krakend-ratelimit) 
KrakenD rate limiter implementation based on GCRA algorithm using github.com/throttled/throttled implementation

## Request and response verifiers and manipulators

1. [krakend-martian](https://github.com/devopsfaith/krakend-martian) injects martian modifiers into the KrakenD proxy pipe
2. [krakend-jsonschema](https://github.com/devopsfaith/krakend-jsonschema) exposes a KrakenD middleware for input validation using JSON schema definitions.
3. [krakend-cel](https://github.com/devopsfaith/krakend-cel) exposes factories for injecting CEL evaluators into the three major pipe parts: endpoint rejected, proxy factory and backend factory.

## Caching

1. [krakend-httpcache](https://github.com/devopsfaith/krakend-httpcache) embeds an in-memory caching system that keeps the responses using the time specified in the Cache HTTP headers.

## Transports

1. [krakend-grpc](https://github.com/devopsfaith/krakend-grpc) contains some experimental bindings for dealing with gRPC backends
2. [krakend-amqp](https://github.com/devopsfaith/krakend-amqp)
3. [krakend-pubsub](https://github.com/devopsfaith/krakend-pubsub)

## Security

### JWT

1. [krakend-jose](https://github.com/devopsfaith/krakend-jose) offers two simple endpoint handlers for signing and verifing JWT
2. [bloomfilter](https://github.com/devopsfaith/bloomfilter/tree/master/krakend) exposes a Rejecter for tokens and cookies using a rotable, distributed and eventualy consistent bloomfilter

### OAuth2 client credentials

1. [krakend-oauth2-clientcredentialst](https://github.com/devopsfaith/krakend-oauth2-clientcredentials) offers a proxy.HTTPClientFactory implementation wrapping the golang.org/x/oauth2/clientcredentials lib

### HTTP

1. [krakend-httpsecure](https://github.com/devopsfaith/krakend-httpsecure) wraps the [github.com/unrolled/secure](http://github.com/unrolled/secure) package

### CORS

1. [krakend-cors](https://github.com/devopsfaith/krakend-cors) wraps the [github.com/rs/cors](http://github.com/rs/cors) package for mux and [gopkg.in/gin-contrib/cors.v1](https://gopkg.in/gin-contrib/cors.v1) package for gin.

### IP filtering

1. [krakend-ipfilter](https://github.com/xiachufang/krakend-ipfilter) IP and CIDR filter middleware to control accesses based on IP

## Log

1. [krakend-gologging](https://github.com/devopsfaith/krakend-gologging) offers an improved logger for the [KrakenD](https://github.com/devopsfaith/krakend) framework by adapting the [github.com/op/go-logging](github.com/op/go-logging) lib
2. [krakend-logrus](https://github.com/devopsfaith/krakend-logrus) offers an improved logger for the [KrakenD](https://github.com/devopsfaith/krakend) framework by adapting the [github.com/sirupsen/logrus](https://github.com/sirupsen/logrus) lib
3. [krakend-logstash](https://github.com/devopsfaith/krakend-logstash) is a log formatter compatible with logstash (uses [krakend-gologging](https://github.com/devopsfaith/krakend-gologging)
4. [krakend-gelf](https://github.com/devopsfaith/krakend-gelf) is a gelf adapter for sending logs to GrayLog, Logstash, etc.

## Config

### Parser

1. [krakend-viper](https://github.com/devopsfaith/krakend-viper) parse config files from multiple formats
2. [krakend-flexibleconfig](https://github.com/devopsfaith/krakend-flexibleconfig) extended features for KrakenD config parsers (variable substitutions, etc)

### Extra

1. [config2dot](https://github.com/devopsfaith/krakend-config2dot) is a tool for translating config files into dot graphs

## CLI

1. [krakend-cobra](https://github.com/devopsfaith/krakend-cobra) integrates the [cobra](github.com/spf13/cobra) lib into the [KrakenD](https://github.com/devopsfaith/krakend) framework
2. [kraki](https://github.com/moritzploss/kraki) is a linter and utility tool for KrakenD config files

## Kubernetes

1. [mikescandy/krakend-helm](https://github.com/mikescandy/krakend-helm) KrakenD Helm chart to install KrakenD on k8s.

## Devel

1. [krakend-memviz](https://github.com/devopsfaith/krakend-memviz) Adds a dotfile exporter of resquest/response snapshots to your proxy stack for debug and devel pourposes (**it will kill your performance**)
2. [krakend-spew](https://github.com/devopsfaith/krakend-spew) Dumps every resquest/response passing through your proxy stacks for debug and devel pourposes (**it will kill your performance**)
3. [krakend-postman](https://github.com/devopsfaith/krakend-postman) Create automatic POSTMAN collection descriptions from you KrakenD config file
4. [hands on krakend](https://github.com/lreimer/hands-on-krakend) Offers examples regarding working with KrakenD plugins

## API Management

1. [krakend-deprecator](https://github.com/moritzploss/krakend-deprecator) is a middleware to schedule and automate endpoint deprecation
