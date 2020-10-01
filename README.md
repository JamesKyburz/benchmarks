<div align="center">
<img src="https://github.com/fastify/graphics/raw/master/full-logo.png" width="650" height="auto"/>
</div>

<div align="center">

[![Build Status](https://travis-ci.org/fastify/fastify.svg?branch=master)](https://travis-ci.org/fastify/fastify)
[![Coverage Status](https://coveralls.io/repos/github/fastify/fastify/badge.svg?branch=master)](https://coveralls.io/github/fastify/fastify?branch=master)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](http://standardjs.com/)
[![NPM version](https://img.shields.io/npm/v/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify)
[![NPM downloads](https://img.shields.io/npm/dm/fastify.svg?style=flat)](https://www.npmjs.com/package/fastify) [![Gitter](https://badges.gitter.im/gitterHQ/gitter.svg)](https://gitter.im/fastify)
</div>
<br />

# TL;DR

* [Fastify](https://github.com/fastify/fastify) is, fast and low overhead web framework for Node.js
* This package shows how fast it is comparatively.

# Installing

```
npm i -g fastify-benchmarks
```

# Usage

```
benchmark [arguments (optional)]
```

#### Arguments

* `-h`: Help on how to use the tool.
* `compare`: Get comparative data for your benchmarks.

> You may also compare all test results, at once, in a single table; `benchmark compare -t`

> You can also extend the comparison table with percentage values based on fastest result; `benchmark compare -p`
# Benchmarks
* __Machine:__ Linux fv-az151 5.4.0-1025-azure #25~18.04.1-Ubuntu SMP Sat Sep 5 15:28:57 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.18.4`
* __Run:__ Thu Oct  1 00:57:19 UTC 2020

|                          | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:    | :-:        | --:     | --:           |
| bare                     | ✗      | 35443.0    | 2.72    | 5.54          |
| connect-router           | ✓      | 29090.8    | 3.34    | 4.55          |
| connect                  | ✗      | 33358.4    | 2.90    | 5.22          |
| egg.js                   | ✓      | 12977.6    | 7.63    | 4.28          |
| express-route-prefix     | ✓      | 6957.6     | 14.24   | 2.42          |
| express-with-middlewares | ✓      | 6473.6     | 15.29   | 2.34          |
| express                  | ✓      | 7498.3     | 13.17   | 1.17          |
| fastify-big-json         | ✓      | 8126.1     | 12.15   | 93.30         |
| fastify                  | ✓      | 34838.0    | 2.77    | 5.45          |
| foxify                   | ✓      | 33636.2    | 2.87    | 4.78          |
| hapi                     | ✓      | 17108.4    | 5.77    | 2.68          |
| koa-router               | ✓      | 21884.9    | 4.48    | 3.42          |
| koa                      | ✗      | 25874.8    | 3.77    | 4.05          |
| micro-route              | ✓      | 28146.4    | 3.45    | 4.40          |
| micro                    | ✗      | 33220.8    | 2.91    | 5.20          |
| microrouter              | ✓      | 19554.8    | 5.02    | 3.06          |
| polka                    | ✓      | 32273.6    | 3.00    | 5.05          |
| polkadot                 | ✗      | 37862.4    | 2.51    | 5.92          |
| rayo                     | ✓      | 32363.2    | 2.99    | 5.06          |
| restify                  | ✓      | 22381.6    | 4.37    | 3.54          |
| server-base-router       | ✓      | 26393.2    | 3.69    | 4.13          |
| server-base              | ✗      | 28682.0    | 3.39    | 4.49          |
| spirit-router            | ✓      | 28433.6    | 3.15    | 4.45          |
| spirit                   | ✗      | 26824.0    | 3.33    | 4.20          |
| take-five                | ✓      | 0.0        | 0.00    | 0.00          |
| total.js                 | ✓      | 22484.0    | 4.34    | 6.39          |
| trek-engine              | ✗      | 23396.0    | 4.18    | 3.32          |
| trek-router              | ✓      | 26280.4    | 3.71    | 3.73          |
| vapr                     | ✓      | 24371.2    | 4.00    | 3.46          |
| yeps-router              | ✓      | 26296.8    | 3.70    | 4.11          |
| yeps                     | ✗      | 28587.6    | 3.40    | 4.47          |
