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
* __Machine:__ Linux fv-az54 5.0.0-1028-azure #30~18.04.1-Ubuntu SMP Fri Dec 6 11:47:59 UTC 2019 x86_64 x86_64 x86_64 GNU/Linux | 2 vCPUs | 7GB.
* __Method:__ `autocannon -c 100 -d 40 -p 10 localhost:3000` (two rounds; one to warm-up, one to measure).
* __Node:__ `v12.14.1`
* __Run:__ Sat Feb  1 00:44:57 UTC 2020

|                          | Router | Requests/s | Latency | Throughput/Mb |
| :--                      | --:    | :-:        | --:     | --:           |
| bare                     | ✗      | 58236.0    | 1.63    | 9.11          |
| connect-router           | ✓      | 50398.4    | 1.89    | 7.88          |
| connect                  | ✗      | 54596.8    | 1.74    | 8.54          |
| egg.js                   | ✓      | 19373.3    | 5.09    | 6.39          |
| express-route-prefix     | ✓      | 29720.8    | 3.25    | 10.35         |
| express-with-middlewares | ✓      | 23553.2    | 4.14    | 8.51          |
| express                  | ✓      | 30364.0    | 3.19    | 4.75          |
| fastify-big-json         | ✓      | 10206.8    | 9.66    | 117.19        |
| fastify                  | ✓      | 60627.2    | 1.56    | 9.48          |
| foxify                   | ✓      | 56287.2    | 1.69    | 8.00          |
| hapi                     | ✓      | 25212.4    | 3.88    | 3.94          |
| koa-router               | ✓      | 36497.4    | 2.66    | 5.71          |
| koa                      | ✗      | 41356.8    | 2.33    | 6.47          |
| micro-route              | ✓      | 49475.2    | 1.93    | 7.74          |
| micro                    | ✗      | 54269.6    | 1.75    | 8.49          |
| microrouter              | ✓      | 28528.8    | 3.40    | 4.46          |
| polka                    | ✓      | 56941.6    | 1.67    | 8.91          |
| polkadot                 | ✗      | 61438.4    | 1.51    | 9.61          |
| rayo                     | ✓      | 55968.8    | 1.70    | 8.75          |
| restify                  | ✓      | 41024.8    | 2.35    | 6.49          |
| server-base-router       | ✓      | 52040.8    | 1.83    | 8.14          |
| server-base              | ✗      | 51020.8    | 1.87    | 7.98          |
| spirit-router            | ✓      | 41247.2    | 1.94    | 6.45          |
| spirit                   | ✗      | 43504.8    | 1.82    | 6.80          |
| take-five                | ✓      | 0.0        | 0.00    | 0.00          |
| total.js                 | ✓      | 39366.4    | 2.45    | 10.29         |
| trek-engine              | ✗      | 47247.2    | 2.03    | 6.71          |
| trek-router              | ✓      | 47468.8    | 2.02    | 6.75          |
| vapr                     | ✓      | 43144.8    | 2.23    | 6.13          |
| yeps-router              | ✓      | 43485.6    | 2.21    | 6.80          |
| yeps                     | ✗      | 51032.0    | 1.87    | 7.98          |
